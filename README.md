# Interitance-OOP-
//example_1:
class Animal {
    void eat() {
        System.out.println("Animal is eating.");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Dog is barking.");
    }
}

public class Main {
    public static void main(String[] args) {

        Dog d = new Dog();

        d.eat();
        d.bark();
    }
}

//example_2:
class Student {
    String name = "Eliyas";

    void study() {
        System.out.println("He is an outgoing student.");
    }
}

class CSEStudent extends Student {
    void programming() {
        System.out.println("He teaches programming.");
    }
}

public class Main {
    public static void main(String[] args) {

        CSEStudent s = new CSEStudent();

        System.out.println("Name: " + s.name);
        s.study();
        s.programming();
    }
}

//example_3:

class Vehicle {
    String brand;
    Vehicle(String brand) {
        this.brand = brand;
    }
    void start() {
        System.out.println("Starting the vehicle.");
    }
}

class Car extends Vehicle {
    int speed;
    Car(String brand, int speed) {
        super(brand);
        this.speed = speed;
    }
    void accelerate() {
        System.out.println("Accelerating to " + speed + " mph.");
    }
}

public class InheritanceExample {
    public static void main(String[] args) {
        Car myCar = new Car("Toyota", 60);
        System.out.println("Car brand: " + myCar.brand);
        
        myCar.start();
        myCar.accelerate();
    }
}
