# Introduction to OOPS
## What is OOPS?

## Procedural Programming vs Object-Oriented Programming
> Procedural programming is about writing procedures or methods that perform operations on the data, by storing state in data structures and behavior in methods/functions.
> While object-oriented programming is about creating objects that contain both data (state) and methods (behaviour) within itself, just like real life objects, having some properties/characteristics and actionable behaviours.

> Procedural Programming is a top-down, step-by-step, function driven approach, based on the concept of procedure(function) call.
State(data) and behavior(logic) are implemented separately. State is stored in data structures and behavior is held in functions.
The data structures are passed as parameters into functions to perform operations on them.

> Object-Oriented Programming is based on classes and objects. It is a bottom-up approach.
State(data) and behavior(logic) are implemented together in the form of objects by using classes.
Objects have state(attributes/data/variables) and behavior(methods/functions) to perform operations on the state.

> Objects are created in heap memory at runtime, using new keyword and constructors.
Classes are created in metaspace out of heap memory at compile time, using class keyword and class definition.

Let's look at examples in both procedural and object-oriented programming to illustrate the difference.

In procedural programming, data structures and methods (functions) are separate. You define data structures and then write functions to perform operations on those data structures. Here's a simple example in C, a procedural programming language:

```c
#include <stdio.h>

// Data structure
struct Student {
    char name[50];
    int age;
};

// Function to print student details
void printStudent(struct Student s) {
    printf("Name: %s\n", s.name);
    printf("Age: %d\n", s.age);
}

int main() {
    struct Student s1 = {"John", 20};
    printStudent(s1);
    return 0;
}
```

In this example, `Student` is a data structure and `printStudent` is a function that operates on a `Student` object. The function is separate from the data structure.

In contrast, in object-oriented programming (OOP), data and methods are encapsulated together in objects. An object is an instance of a class, and a class defines both data (attributes) and methods. Here's a similar example in Java, an object-oriented programming language:

```java
public class Student {
    String name;
    int age;

    // Constructor
    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Method to print student details
    public void printStudent() {
        System.out.println("Name: " + this.name);
        System.out.println("Age: " + this.age);
    }

    public static void main(String[] args) {
        Student s1 = new Student("John", 20);
        s1.printStudent();
    }
}
```

In this example, `Student` is a class that encapsulates the data (`name` and `age`) and the method (`printStudent`) together. The method is part of the object, and it can directly access the object's data.

## Advantages of OOPS:
> Re-usability: Through classes and objects, and inheritance of common attributes and functions.

> Security: Hiding and protecting information through encapsulation.

> Maintenance: Easy to make changes without affecting existing objects much.

> Inheritance: Easy to import required functionality from libraries and customize them, thanks to inheritance.


## Disadvantages of OOPS:
> Beforehand planning of entities that should be modeled as classes.

> OOPS programs are usually larger than those of other paradigms.

> Banana-gorilla problem - You wanted a banana but what you got was a gorilla holding the banana and the entire jungle


## Principle and Pillars of OOPS:
### ABSTRACTION - Principle of OOPS:
_Process of hiding the implementation details and showing only functionality to the user._

Abstraction lets you focus on what the object does instead of how it does it.

### Pillars of OOPS:
_Pillar 1 - ENCAPSULATION:_ 
> Wrapping up of data (state) and methods (behavior) together into a single unit (i.e. class) and also hiding the data from outside world (i.e. data hiding).

_Pillar 2 - INHERITANCE:_ 
> Process by which one class acquires the properties of another class (i.e. re-usability).

_Pillar 3 - POLYMORPHISM:_ 
> Ability of a message to be displayed in more than one form (i.e. method overriding and method overloading).

*Call by Value vs Call by Reference*
-
1. >Call by Value: Passing the value of the variable as an argument, so that the parameter is initialized with the value of the variable.
2. >Call by Reference: Passing the address of the variable as an argument, so that the parameter is initialized with the address of the variable.

   > Java supports only Call by Value.

*Types of Variables:*
-
1. >Primitive Variables
2. >Reference Variables
3. >Static Variables
4. >Instance Variables or Non-Static Variables
5. >Final Variables
6. >Local Variables
7. >Global Variables

*Types of Methods:*
-
1. >Static Methods
2. >Instance Methods or Non-Static Methods
3. >Final Methods
4. >Abstract Methods
5. >Synchronized Methods
6. >Native Methods
7. >Default Methods
 
*List of Keywords in Java:*
-
1. >abstract
2. >this
3. >super
4. >static
5. >final
6. >new
7. >return
8. >void
9. >public
10. >private
11. >protected
12. >default
13. >class
14. >interface
15. >extends
16. >implements
17. >package
18. >import
19. >throws
20. >throw
21. >try
22. >catch
23. >finally