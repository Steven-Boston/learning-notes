# Reading 401-01: Exeption Handling

## Microsoft Docs: How to Debug
This article is available [here](https://docs.microsoft.com/en-us/visualstudio/debugger/debugging-absolute-beginners?view=vs-2019&tabs=csharp).

This article is a breakdown of the debugging process. Much of it retreads territory covered better in the prework readings, but there are a few key points that it takes as its framework: 

- Ask questions about the error, and determine the extent of the unwanted results. 
- Analyze your assumptions about what you wrote, and look for weak points. 
- Use debugging mode to gradually advance your code to pinpoint the bug. 

## Microsoft Docs: Try/Catch blocks
This article is available [here](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions).

Just like in Javascript, Try/Catch is a handy way to deal suspicious code. C# is anything but dull when it comes to the details, though. This means that some more verbose syntax will be required (Imagine my shock). 
```C#

try 
{
  //suspicious stuff
}
catch (SpecificException e)
{
  //error messsage/code
}
catch (OtherSpecificException e)
{
  //message/code for other error
}
```

## Statement Keywords for C#:
This document is pure link hub, and is aviailable [here](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/statement-keywords).

## Therac-25 and Ariane 5:

These wikipedia articles each cover historical issues of programs having unwanted results with serious consequences. They thereby stress the importance of having a strong methodology when approaching coding tasks and using a workflow that makes it easy to approach these kinds of problems. 


[<<Return to Home](../README.md)