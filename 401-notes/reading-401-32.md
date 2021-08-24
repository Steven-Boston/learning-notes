# Reading 401-32: View Components

## Microsoft Docs: View Components
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/view-components?view=aspnetcore-2.1).

View components are a subdivision of the usual view used in MVC and Razor pages. A view component is given its own data to work with when called, and can be used to model some commonly needed component for multiple pages. 

A view component can be initiated with annotations, derivation, or the suffix ViewComponent in the classname. 

The remainder of this documentation covers specific scenarios related to view components, with code samples. 

## Marius Schulz: View Components in ASP.NET Core MVC
This article is available [here](https://mariusschulz.com/blog/view-components-in-asp-net-core-mvc).

Marius goes step by step through the process of useing view components, and there are several steps to be had: 

- Creating a class that inherits `ViewComponent`
- using `@Component.Invoke("name")` to bring the component into the page
- declaring model classes to be used to import data. 
- using dependency injection to enhance functionality.

 A view component is a useful tool for small-but-still-high-functioning pieces of pages. They can be implemented with most of the useful functions available to full views, but have the agility to be used in many contexts. 