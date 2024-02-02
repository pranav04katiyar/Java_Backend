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
> Here the fly() and the sound() methods are handling more than one responsibility:
> - They are handiling 