# Reading 401-31: Razor Pages

## Microsoft Docs: Intro to Razor Pages
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/razor-pages/?view=aspnetcore-2.2&tabs=visual-studio).

Razor pages are a framework for handling a web app from the server. The system consists of cshtml pages that have a razor page .cs file attached to them. This attached file holds the code that will run when it comes time to render the page. 

The code file will generally contain a model for data to be sent to the page, as well as an OnGet() method and possibly an OnPost() method or other supprorting code. Model binding can be used to supply a structure for sending formdata as well (a good use for an OnPost() method). 

This documentation has many additional examples for different situations that can come up with razor pages, such as configuration, multiple handlers, custom routes, and more. 

## Gunnar Peipman: RAzor Pages with ASP.NET core 2
This article is available [here](https://gunnarpeipman.com/aspnet-core-razor-pages/).

Gunnar opens this article with a section on why one would choose Razor pages: 

- razor pages are lightweight, which creates ease of use on smaller endeavors
- razor pages are less obtuse for beginners

The rest of the article takes the opposite position: that the percieved ease of use and lighter requirements are not particularly prohibitive, and that having so carefully subdivided code for each page can become somewhat cumbersome (an idea with which I sympathize). He also provides some explanation of the basic procedures in razor pages from the perspective of an MVC developer. 

## Jon Hilton: Razor Pages vs. MVC
This article is available [here](https://jonhilton.net/razor-pages-or-mvc-a-quick-comparison/).

MVC and Razor pages are two competing systems in the arena of creating server side web apps in .NET. This make it useful to compare the two directly:

- MVC handles routing through controllers, which generally return views, which are created from markup files with corresponding names. 
- Razor Pages route to the markup, which has a razor page attached to it as `@page`. The razor page contains methods that provide a model for the page data. 

Jon concludes by pointing out that MVC isn't going anywhere, and continues to recieve updates.

[<<Return to Home](../README.md)