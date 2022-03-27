## Inheritance

Inheritance allows us to define a class in terms of another class, which makes it easier to create and maintain an application. This also provides an opportunity to reuse the code functionality and speeds up implementation time.
When creating a class, instead of writing completely new data members and member functions, the programmer can designate that the new class should inherit the members of an existing class. This existing class is called the base class, and the new class is referred to as the derived class.
The idea of inheritance implements the IS-A relationship. For example, mammal IS A animal, dog IS-A mammal hence dog IS-A animal as well.
 Example:-
 ![b259eb1ece0c5ec37d17638ee590ebd0](https://user-images.githubusercontent.com/98957434/160265335-d4357c2d-d03b-481d-8d6f-646705d21743.png)



## Abstract

There are situations in which we want to define a superclass that declares the structure of a given abstraction without providing a complete implementation of every method. That is, sometimes we want to create a superclass that only defines a generalized form that will be shared by all of its subclasses, leaving it to each subclass to fill in the details.

abstract class Shape {
 
    public abstract int area();
}

class Square : Shape {


## Polymorphism

means providing an ability to take more than one form and it’s one of the main pillar concepts of object-oriented programming, after encapsulation and inheritance. Generally, the polymorphism is a combination of two words, one is poly and another one is morphs.

![th (1)](https://user-images.githubusercontent.com/98957434/160265453-f042472e-ce76-493a-a759-5d61f196a814.jpg)


## OOP Principles

The Object Oriented programming paradigm plays an important role in human computer interface. It has different components that takes real world objects and performs actions on them, making live interactions between man and the machine.
This paradigm describes a real-life system where interactions are among real objects.
It models applications as a group of related objects that interact with each other.
The programming entity is modeled as a class that signifies the collection of related real world objects.
components of object oriented programming.
