# Reading 401-08: Collections and Enums

## Microsoft Docs: Collections
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections).

Collections offer an alternative to arrays for storing groups of data. Collections are classes, and can be instantiated just like other classes:

```C#
var cards = new List<string>();
cards.Add("The Scarab God");
cards.Add("Snapcaster Mage");
cards.Add("Overgrown Tomb");
```
or:

```C#
var cards = new List<string> {
  "The Scarab God",
  "Snapcaster Mage",
  "Overgrown Tomb"
};
```

The above codeblocks make lists of strings, but the list could be of any type, even custom classes. The documentation on collections also gives an overview of other types of collections, up to and including fully custom collections. 

## Microsoft Docs: Enumeration Types 
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum).

enum, or the **enumeration type**, allows for data to be stored with a logical progression of numerical keys. These keys can use a default sequence or be manually defined. This allows us to store odd types of data and access them easily. 

We can also use casting to convert values in an enum into their corresponding integers with `(int)x`, allowing for a level of reverse-referencing. 


[<<Return to Home](../README.md)