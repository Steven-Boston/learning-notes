# Reading 401-04: Classes and Memory Management

## Microsoft Docs: Introduction to Classes
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/classes).

This document focuses on introducing classes for C#. A class is declared with access, `class`, and an identifier, like `public class archeops`. From there we can establish the body of the class, which can contain various methods and properties of the class, as well as anything else that needs to be done to set it up, like the constructor method. 

Classes are also capable of inheritance in C# meaning that a class can be based off of another but have its own divergent methods and proprties. The form for this is `public class newClass : oldClass`.

## Microsoft Docs: Constructors
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/constructors).

The constructor function of a class controls how the class is initialized when a new instance is declared. If none is present, C# will automatically create a default constructor to facilitate the establishment of new instances. A constructor is written as a method with the same name as the class, with only parameters besides name and access scope. Within the constructor the parameters can be used in order to arrange the data and functionality of the instance. 

## Microsoft Docs: Properties
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/properties).

Properties are a method whose main set of functionality is to manage a partcular set of data within the class. A property often has `get` and `set` accessors that allow for the value within to be easily accessed of changed, but may also have init rather than set if the value needs to be locked at initialization. It is possible the use the property method and the accessors in order to control access in a property as well.

## Matthew CochranL Heap vs. Stack
This article is available [here](https://www.c-sharpcorner.com/article/C-Sharp-heaping-vs-stacking-in-net-part-i/).

The computer science system is made up of two units: The stack, which keeps track of the list of running processes, and the heap, which tracks the objects present in those locations. These are their stories. 

The stack and the heap both deal with how memory is assigned to the running of our applications, and understanding their interactions is critical to being able to manipulate our efficiency effectively. The core concept surrounding these is that they have to both keep track of the values that we have created and assigned as well as manage references that connect everything properly tied together. All of this has a cost in memory, so it is critical that we are able to keep track of each additional item and ensure it is needed. 

## Microsoft Docs: Fundamentals of Garbage Collection
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/fundamentals).

The heap has an important role that we as C# developers luckily needn't directly concern ourselves with: Garbage Collection. Garbage collection can be explained as the process by which the heap dismisses unnecessary references to vestigial values. This is the process by which variables are cleared once we have exited their scope. The documentation above provides a detailed breakdown of the algorithm by which the CLR determines how and when to act. 


[<<Return to Home](../README.md)