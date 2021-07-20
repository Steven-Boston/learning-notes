# Reading 401-07: Interfaces

## Microsoft Docs: Interfaces 1 & 2
These documents are available [here](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/interfaces) and [here](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/interface).

An interface could be roughly described as a way to standardize the usage and behavior of some group of classes, in order to be able to utilize them easily. Interfaces are especially valuable in C# because they are the most straightforward way of bringing disparate classes together to form a singular implementation. 

`interface IDoStuff { }` is the form for creating an interface, which generally always have a name beginning with a capital I. Within the brackets we can define public members for the interface, which inheriting classes will required to implement. In this way, an interface is essentially a class that behaves as if everything in it lives with an abstract tag, and then forces those things upon its descendants. 

## John Sonmez: What is an Interface?
This article is available [here](https://simpleprogrammer.com/back-to-basics-what-is-an-interface/).

John begins with a declaration: 

> "The basic problem an interface is trying to solve is to separate how we use somthing from how it is implemented."

This boils down to a question of utility. An interface is tasked with providing the developer with a shield from the inner workings of our programs. No one wants to know where that boolean gets changed, how we derive that string, of the damage formula that determines what their hammer does. 

Given this, it becomes important to consider: are interfaces being used correctly? do they simplify code by binding things together, or simply provide an additional level of mud to facilitate unit testing?

