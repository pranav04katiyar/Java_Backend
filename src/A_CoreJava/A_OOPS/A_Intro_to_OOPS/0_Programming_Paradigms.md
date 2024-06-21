# Introduction to OOPS(Object-Oriented Programming System)
## LLD: Low Level Design
Low-level design (LLD) is a component-level design process that follows a step-by-step refinement process to provide the internal logical design of the actual program code.

To put it in simple terms, LLD is the process of telling the system how the software will be implemented.

LLD has the following goals:
> 1. Low level implementation details of a system
> 2. Organization of code
> 3. Writing good software

### *What is a good software?*
A good software is a software that is:
1. >Easy to understand 
2. >Easy to maintain: Modular(loosely coupled, high cohesion), Reusable, Analyzable, Modifiable, Testable
3. >Easy to scale: Adaptable, Efficient, Reliable, Secure, can increase capacity and functionality as per the requirement.
4. >Easy to extend: Flexible, Effortlessness in adding new features, Enhanceable without breaking existing features. 

#### *Extensibility vs Scalability:*
Extensibility is the ability to add new features without breaking existing features - Capability(Feature functionality) based.

Scalability is the ability to increase capacity and functionality as per the requirement - Performance(Usage demand) based.

## Programming Paradigms:

> Imperative Programming: focuses on describing how a program operates (algorithm) by providing a set of well-defined instructions to change state(data).
  Example: Procedural Programming(Eg: C,COBOL,BASIC,FORTRAN etc), Object Oriented Programming(Eg: Java,C++,C#,Python etc)

> Declarative Programming: focuses on describing what a program should accomplish without specifying how the program should achieve the result.
  Example: SQL, HTML, CSS, XML, Functional Programming(Eg: Haskell, Lisp, Erlang, Clojure etc), Logic Programming(Eg: Prolog, Datalog etc)

Procedural Programming vs Object-Oriented Programming:
-
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
 
Advantages of OOPS over Procedural Programming:

> Re-usability: Through classes and objects, and inheritance of common attributes and functions.

> Security: Hiding and protecting information through encapsulation.

> Maintenance: Easy to make changes without affecting existing objects much.

> Inheritance: Easy to import required functionality from libraries and customize them, thanks to inheritance.

Disadvantages of OOPS over Procedural Programming:

> Beforehand planning of entities that should be modeled as classes.

> OOPS programs are usually larger than those of other paradigms.

> Banana-gorilla problem - You wanted a banana but what you got was a gorilla holding the banana and the entire jungle
