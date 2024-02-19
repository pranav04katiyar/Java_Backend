*Single Responsibility Principle*
-
> SRP states that "A class should have only one reason to change, meaning that a class should have only one job."

> In the previous code, the methods in the Bird class has multiple responsibilities, which means they need to change for more than one reason:
>  - Let's say there are many types of birds with their unique flying styles and sounds:
```Java
public void fly() {
    if (type.equals(sparrow)) {
        System.out.println("Sparrow is flying");
    }
    if (type.equals(pigeon)) {
        System.out.println("Pigeon is flying");
    }
    if (type.equals(crow)) {
        System.out.println("Crow is flying");
    }
}

public void eat(){
    if(type.equals(sparrow)){
        System.out.println("Sparrow is eating");
    }
    if(type.equals(pigeon)){
        System.out.println("Pigeon is eating");
    }
    if(type.equals(crow)){
        System.out.println("Crow is eating");
    }
}

public void sound(){
    if(type.equals(sparrow)){
        System.out.println("Coo");
    }
    if(type.equals(pigeon)){
        System.out.println("Guter");
    }
    if(type.equals(crow)){
        System.out.println("Kaow");
    }
}
```
> Here the fly(), eat() and the sound() methods are handling more than one responsibility:
> - They are handling the responsibility of flying different types of birds.
> - They are handling the responsibility of eating different types of birds.
> - They are handling the responsibility of making different sounds of birds.

> Hence, there are multiple reasons to change the Bird class:
> - If a new type of bird is added, the fly(), eat() and sound() methods need to be changed.
> - If the flying style, eating style or sound of a bird is changed, the fly(), eat() and sound() methods need to be changed.

> This is a violation to the Single Responsibility Principle.

> Along with this, there are multiple other issues with this Bird class:
> - Readability: The code is not readable and maintainable. If we add more types of birds, the code will become more complex.
> - Testability: We cannot test the fly(), eat() and sound() methods separately for each type of bird as they are in the same class.
> - Parallel Development: We cannot develop the fly(), eat() and sound() methods in parallel as they are in the same class.

> To solve this, 
```Java
public class Bird {
    private double weight;
    private String color;
    private String size;
    private String beakType;
    private String typeOfBird;

    public void fly() {
        if (type.equals(sparrow)) {
            flyLikeSparrow();
        }
        if (type.equals(pigeon)) {
            flyLikePigeon();
        }
        if (type.equals(crow)) {
            flyLikeCrow();
        }
    }

    public void eat() {
        if (type.equals(sparrow)) {
            eatLikeSparrow();
        }
        if (type.equals(pigeon)) {
            eatLikePigeon();
        }
        if (type.equals(crow)) {
            eatLikeCrow();
        }
    }

    public void sound() {
        if (type.equals(sparrow)) {
            soundLikeSparrow();
        }
        if (type.equals(pigeon)) {
            soundLikePigeon();
        }
        if (type.equals(crow)) {
            soundLikeCrow();
        }
    }
}
```