# Reading 401-14: Routing and Navigation

## Microsoft Docs: MVC Routing Overview
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/controllers-and-routing/asp-net-mvc-routing-overview-cs).

Routing is the process of taking a web request and determining the correct control functions to run as a response. The default controller that is present in all MVC applications has a basic routing by id function that is put in place on startup. This can be connected to a controller to provide some level of optionality, but it is hardly ideal. 

## Microsoft Docs: Routing in ASP.NET Core
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/routing?view=aspnetcore-3.1).

One might rightly suspect that a better way to manage requests must exist. In ASP.NET core, routing can be handled via endpoints. These endpoints can be manually defined to map to specific functions, and given their own unique signature for access. This arms the developer with a bevy of versatile tools with which to handle a variety of requests to their API. 

[<<Return to Home](../README.md)