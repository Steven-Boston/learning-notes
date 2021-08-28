# Reading 401-27: Forms

## Microsoft Docs: Views in ASP.NET Core MVC
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/overview?view=aspnetcore-2.2).

When building a web app with MVC (model view controller), the views are the files from which your site's appearance is sourced. This manifests in the form of HTML that has been augmented with Razor Markup form C#. 

MVC summons views via controllers, which have methods within them that call the views. In order for this to line up, the file structure should be such that the views are in a views folder, which has within it a folder bearing the name of the controller, within which the view is contained. Returning View() from the corresponding method will look for the view file at that location.

## Complete C#: Creating Forms in MVC
This Article is available [here](https://www.completecsharptutorial.com/asp-net-mvc5/4-ways-to-create-form-in-asp-net-mvc.php).
[<<Return to Home](../README.md)

In MVC a form has the basic skeleton of a standard HTML form, with Razor markup added to link the form to a model. The form tag is given razor markup that directs the submit to a particular controller and action, where the model created by the controller can be processed. 

The article outlines a few different approaches to accomplish this depending on the circumstances and language availability, complete with code examples. 
