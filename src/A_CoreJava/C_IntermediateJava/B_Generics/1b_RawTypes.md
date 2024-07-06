# Raw Types

A raw type is the name of a generic class or interface without any type arguments. For example, given the generic Box class:
````
public class Box<T> {
public void set(T t) { /* ... */ }
//...
}
````
To create a parameterized type of Box<T>, you supply an actual type argument for the formal type parameter T:
````
Box<Integer> intBox = new Box<>();
````
If the actual type argument is omitted, you create a raw type of Box<T>:
````
Box rawBox = new Box();
````
Therefore, Box is the raw type of the generic type Box<T>. However, a non-generic class or interface type is not a raw type.

Raw types show up in legacy code because lots of API classes (such as the Collections classes) were not generic prior to JDK 5.0. When using raw types, you essentially get pre-generics behavior — a Box gives you Objects. For backward compatibility, assigning a parameterized type to its raw type is allowed:
````
Box<String> stringBox = new Box<>();
Box rawBox = stringBox;               // OK
````
But if you assign a raw type to a parameterized type, you get a warning:
````
Box rawBox = new Box();           // rawBox is a raw type of Box<T>
Box<Integer> intBox = rawBox;     // warning: unchecked conversion
````
You also get a warning if you use a raw type to invoke generic methods defined in the corresponding generic type:
````
Box<String> stringBox = new Box<>();
Box rawBox = stringBox;
rawBox.set(8);  // warning: unchecked invocation to set(T)
````
The warning shows that raw types bypass generic type checks, deferring the catch of unsafe code to runtime. Therefore, you should avoid using raw types.

The Type Erasure section has more information on how the Java compiler uses raw types.

### Unchecked Error Messages

As mentioned previously, when mixing legacy code with generic code, you may encounter warning messages similar to the following:

Note: Example.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
This can happen when using an older API that operates on raw types, as shown in the following example:
````
public class WarningDemo {
public static void main(String[] args){
Box<Integer> bi;
bi = createBox();
}

    static Box createBox(){
        return new Box();
    }
}
````
The term "unchecked" means that the compiler does not have enough type information to perform all type checks necessary to ensure type safety. The "unchecked" warning is disabled, by default, though the compiler gives a hint. To see all "unchecked" warnings, recompile with -Xlint:unchecked.

Recompiling the previous example with -Xlint:unchecked reveals the following additional information:

WarningDemo.java:4: warning: [unchecked] unchecked conversion
found   : Box
required: Box<java.lang.Integer>
bi = createBox();
^
1 warning
To completely disable unchecked warnings, use the -Xlint:-unchecked flag. The @SuppressWarnings("unchecked") annotation suppresses unchecked warnings.