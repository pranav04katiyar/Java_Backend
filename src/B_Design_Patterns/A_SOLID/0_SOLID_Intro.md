*SOLID*
-
> It is an acronym for five design principles intended to make software designs more understandable, flexible, and maintainable. It is a subset of Object-Oriented Design Principles.

> The five principles are:
>   - Single Responsibility Principle
>   - Open Closed Principle
>   - Liskov Substitution Principle
>   - Interface Segregation Principle
>   - Dependency Inversion Principle

> We will discuss each of these principles in detail with the help of an example - Designing a Bird.

- > A bird has the following properties and methods:
  - Weight
  - Color
  - Size
  - BeakType
  - TypeOfBird
  - Fly()
  - Eat()
  - Sound()

> Let's code the initial version of the Bird class:
```Java
public class Bird {
    private double weight;
    private String color;
    private String size;
    private String beakType;
    private String typeOfBird;

    public void fly() {
        System.out.println("Bird is flying");
    }

    public void eat() {
        System.out.println("Bird is eating");
    }

    public void sound() {
        System.out.println("Bird is making sound");
    }
}
```