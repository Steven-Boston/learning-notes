# Reading 301-10: In Memory Storage

## Understanding the Call stack
This article by Charles Freeborn is available [here](freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

This article describes the rules that govern the call stack- the order by which JavaScript resolves competing tasks. Javascript does this in Last-In, First-Out fashion, resulting in an order of execution that can seem counterintuive, but follows a simple sort of logic. This becomes important anytime we operate our functions asynchronously. 
 
## JavaScript Error Messages
This article  by Diogo Spinola is available [here](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

This article is a breakdown of errors in JavaScript. I covers both the different types of errors as well a modicum of ways to handle them. There are several types of errors that we will commonly encounter when working with JavaScript: 

- Reference Errors
  * Indicate an issue witha variable reference, such as it not having been declared
- Syntax Errors
  * A flaw in the syntax that is preventing the code from running. 
- Range Errors
  * Some iterable has had its range manually changed. In invalid fashion. 
- Type Errors
  * The type of variable you are using does not line up with what you are using it for. 

The article then goes over some common process for debugging: Use console logs and other marker to pinpoint the problem, then write the code to solve it. This can involve a number of troubleshooting steps and some mild detective work. 

#### Additional Bookmarks

[JavaScript Error Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

[<<Return to Home](../README.md)