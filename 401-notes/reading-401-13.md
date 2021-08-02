# Reading 401-13: Dependency Injection and Repository Design

## Microsoft Docs: Dependency Injection in ASP.NET
This documentation is available [here]().

Dependency injection is the process of rerouting a task to a custom handler by using an instance of the desired handler and substituting it wherever the default handler would be necessary. This can be applicable in a variety of scenarios, and many of them are outlined in detail in this documentation. 

## Microsoft Docs: Designing the Infrastructure Persistence Layer
This documentation is available [here]().

This document overviews best practices for overall design in terms of handling a breadth of data stored in multiple clusters of tables. It has once basic idea: each repository should serve only one cluster of tables. This both enables more efficient testing and allows for easier updates to the individual clusters should the need arise. 

## Per-Erik Bergman: Repository Design Pattern
This article is available [here]().

This article disusses the use of repository design in setting Data Access Objects for our models. In particular, it compares the idea of using a single multipurpose set of CRUD methods that covers the handling for each model versus the repository pattern of having a common control pattern and subdividing the tasks. Keeping each item smaller and easier to parse make the correct option quite clear indeed.

## SOLID Principles
This article is available [here](https://www.telerik.com/blogs/30-days-of-tdd-day-five-make-your-code-solid).
## Why SOLID Matters
This article is available [here](https://www.telerik.com/blogs/why-solid-matters).

SOLID is a set of principles that outline how class (and thereby program) design should be executed. There are five of these: 

- Single Responsibility: Each class should have a sungular purpose.
- Open-Closed: A finished class can be extended, but should never be modified. 
- Liskov Substutution: A subclass should cover all the functionality of its parent class.
- Interface Segregation: Make separate interfaces to serve individual purposes
- Dependency Inversion: Depend on the abstracts you know your concrete class will have. 

These principles allow us to keep problems compartmentalized and fix them without causing more. They also make it easier (and provide a plan for) adding new features. 

## SOLID Pictures
This article is available [here](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898). It is a series of pictures. 


[<<Return to Home](../README.md)