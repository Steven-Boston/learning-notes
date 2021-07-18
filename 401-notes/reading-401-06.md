# Reading 401-06: OOP Principles

## Microsoft Docs: Inheritance
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/inheritance).

Inheritance is the process of taking a base class and using its default behaviors and data and altering them to create a derived class. This is useful for representing something that is a subcategory of something else. the Rogue class might have a class called swashbuckler derived from it. 

Methods in the base class might be declared as `abstract` or `virtual`, which control how descendant classes must interact with them. More in this in Polymorphism below. A class can also prevent itself from being the target of inheritance using `sealed` in its declaration.

## Microsoft Docs: Abstract and Sealed Classes
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members).

Declaring an abstract class `public abstract class Rogue` is used to create a class that does not have instances, and instead is used to create derivations, possibly through multiple levels of abstraction. This allows for the developer to zero in on the precise subclass features that will be needed. 

As mentioned above, `sealed` forms the opposite end of this idea. A sealed class is disallowed as a base for other classes. `sealed` can also be used for class members to restrict them from further derivations. 

## Microsoft Docs: Polymorphism
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/polymorphism).

It is important to keep in mind how members inherited from the base class will be treated when interacting with matters on class inheritance. `virtual` methods can be transformed- maintaining their virutal status or otherwise in the derived class. 

## Microsoft Docs: OOP Principles
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/tutorials/oop).

Thia documentation covers the four basic principles of object-oriented-programming:

- Abstraction: Taking some entity and building an object that represents it in code. 
- Encapsulation: Defining a set of rules by which the properties of the abstraction may be interacted with
- Inheritance: Use previous representations to create a relative representation of a similar entity. 
- Polymorphism: Control the flow of inheritance over multiple streams of inheritance. 

[<<Return to Home](../README.md)