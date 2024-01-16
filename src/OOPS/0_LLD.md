#This package is about understanding concepts of OOPS in Java.

LLD:
Low-level design (LLD) is a component-level design process that follows a step-by-step refinement process to provide the internal logical design of the actual program code.
LLD has the following goals:
    -> Low level implementation details of a system
    -> Organization of code
    -> Writing good software

*_What is a good software?_*
A good software is a software that is:
    -> easy to understand
    -> easy to maintain: Modular(loosely coupled, high cohesion), Reusable, Analyzable, Modifiable, Testable
    -> easy to scale: Adaptable, Efficient, Reliable, Secure, can increase capacity and functionality as per the requirement.
    -> easy to extend: Flexible, Effortlessness in adding new features, Enhanceable without breaking existing features.

*_Extensibility vs Scalability:_*
Extensibility is the ability to add new features without breaking existing features - Capability(Feature functionality) based.
Scalability is the ability to increase capacity and functionality as per the requirement - Performance(Usage demand) based.

*Programming Paradigms:*
    
    > Imperative Programming: focuses on describing how a program operates (algorithm) by providing a set of well-defined instructions to change state(data).
      Example: Procedural Programming(Eg: C,COBOL,BASIC,FORTRAN etc), Object Oriented Programming(Eg: Java,C++,C#,Python etc)

    > Declarative Programming: focuses on describing what a program should accomplish without specifying how the program should achieve the result.
      Example: SQL, HTML, CSS, XML, Functional Programming(Eg: Haskell, Lisp, Erlang, Clojure etc), Logic Programming(Eg: Prolog, Datalog etc)

Procedural Programming vs Object-Oriented Programming:
    
    > Procedural Programming is a top-down, step-by-step, function driven approach, based on the concept of procedure(function) call.
      State(data) and behavior(logic) are implemented separately. State is stored in data structures and behavior is held in functions.
      The data structures are passed as parameters into functions to perform operations on them.
       
    > Object-Oriented Programming is based on classes and objects. It is a bottom-up approach.
      State(data) and behavior(logic) are implemented together in the form of objects by using classes.
      Objects have state(attributes/data/variables) and behavior(methods/functions) to perform operations on the state.
    
    > Objects are created in heap memory at runtime using new keyword and constructors.
      Classes are created in metaspace out of heap memory at compile time using class keyword and class definition.