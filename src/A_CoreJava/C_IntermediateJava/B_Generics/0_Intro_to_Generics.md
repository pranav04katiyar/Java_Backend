# Generics
Generics enable types (classes and interfaces) to be parameters when defining classes, interfaces and methods. 
- Purpose is to create a class general enough to handle any type of data, while still maintaining compile-time safety.
- Generics allow us to parameterize the attributes of classes and methods.

###### Side Note: Every class in Java is a subclass of the Object class. For example:
> Object obj = new Object(); // Object class reference and object creation
> Object obj = new String("Hello"); // Object class reference and String object creation, as String is a subclass of Object
> Object obj = new Integer(100); // Object class reference and Integer object creation, as Integer is a subclass of Object
> Object obj = new Main(); // Object class reference and Main object creation, as Main is a subclass of Object

### Why use Generics?
There are times when we want the flexibility of using different data types in our classes and methods, without having to create multiple classes or methods to handle each data type. This is where generics come in.

Code that uses generics has many benefits over non-generic code:
1. **Stronger type checks at compile time:**
- Compile-time bugs, can be detected early on, where the compiler's error messages can be used to figure out what the problem is and fix it, right then and there. 
- Runtime bugs, however, can be much more problematic, as they don't always surface immediately, and when they do, it may be at a point in the program that is far removed from the actual cause of the problem.
- > A Java compiler applies strong type checking to generic code and issues errors if the code violates type safety. Fixing compile-time errors is easier than fixing runtime errors, which can be difficult to find.
- Generics add stability to your code by making more of your bugs detectable at compile time.
2. **Elimination of casts:**
- The following code snippet without generics requires casting:
```
List list = new ArrayList();
list.add("hello");
String s = (String) list.get(0);
```
- Whenever we typecast, we are essentially telling the compiler that we know what we are doing and that it should trust us. However, if we make a mistake in our typecast, the compiler will not be able to catch it, and we will get a runtime error.
- When re-written to use generics, the code does not require casting:
```
List<String> list = new ArrayList<String>();
list.add("hello");
String s = list.get(0);   // no cast
```
3. **Enabling programmers to implement generic algorithms:**
- By using generics, programmers can implement generic algorithms that work on collections of different types, can be customized, and are type safe and easier to read.

### Topics to be covered:
- Generic Types & Raw Types
- Generic Classes
- Generic Methods
- Bounded Type Parameters
- Wildcards
- Type Erasure
- Restrictions on Generics