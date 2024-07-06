# Generics
In a nutshell, generics enable types (classes and interfaces) to be parameters when defining classes, interfaces and methods. 
- Much like the more familiar formal parameters used in method declarations, type parameters provide a way for you to re-use the same code with different inputs. The difference is that the inputs to formal parameters are values, while the inputs to type parameters are types.

Code that uses generics has many benefits over non-generic code:

1. **Stronger type checks at compile time:**
- Compile-time bugs, can be detected early on, where the compiler's error messages can be used to figure out what the problem is and fix it, right then and there. 
- Runtime bugs, however, can be much more problematic, as they don't always surface immediately, and when they do, it may be at a point in the program that is far removed from the actual cause of the problem.
- > A Java compiler applies strong type checking to generic code and issues errors if the code violates type safety. Fixing compile-time errors is easier than fixing runtime errors, which can be difficult to find.

Generics add stability to your code by making more of your bugs detectable at compile time.
2. **Elimination of casts:**
- The following code snippet without generics requires casting:
```
List list = new ArrayList();
list.add("hello");
String s = (String) list.get(0);
```
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