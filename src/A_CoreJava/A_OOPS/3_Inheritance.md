*Pillar 2: INHERITANCE -*
-
>Process by which one class acquires the properties of another class (i.e. re-usability)/Ability to copy fields and methods from one class to another class.

_How Inheritance implements OOPS concept:_
-
1. Code Re-usability - Re-use the code of parent class in child class
2. Extensibility - Add more features to the child class
3. Flexibility - Change the code in one place (i.e. parent class) and use it in multiple places (i.e. child class)
4. Modularity - Divide the code into multiple classes and use it in multiple places.

_Concepts in Inheritance:_
-
1. Parent and Child Classes (Super and Sub Classes) - IS-A Relationship
- > extends keyword 
- > super keyword and super() method - constructor chaining
- > this keyword and this() method - constructor telescoping
2. Types of Inheritance:
- > Single Inheritance
- > Multi-Level Inheritance
- > Hierarchical Inheritance
- > Multiple Inheritance (Not supported in Java)
- > Hybrid Inheritance (Not supported in Java) - Combination of Hierarchical and Multiple Inheritance - Diamond Problem
3. Interface - Blueprint of a behavior, contract for implementing classes, 100% abstraction, loose coupling
- > implements keyword
- > Interface for Diamond Problem
4. Abstract Class - A combination of interface and concrete class. Used to achieve partial abstraction(0-100%) & loose coupling.
- > abstract keyword & abstract method
- > default keyword & default method   
5. Interview Questions:    
- > abstract class vs interface/concrete class(default,private,protected,public)/final class
- > abstract method vs final method/static method/concrete method(default,private,protected,public)
- > abstract class vs abstract method
- > abstract class/abstract method vs constructor