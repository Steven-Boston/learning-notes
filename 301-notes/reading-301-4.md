# Reading 301-4: REact and Forms

## React Docss: Forms
This document is available [here](https://reactjs.org/docs/forms.html)

This document is a breakdown of how to implement forms with react, which by their nature must have the ability to maintain some internal state to function, passing that state data to their corresponding handlers to manipulate it. This is generally done by preparing the handler functions within the component that contains the form in question. We can set the value of the input field to correspond to the desired state to be changed, and then make our handler function update that state when the form detects a change event. 

The remainder of the documentation breaks down several other options for forms in react: 

- textarea tags
- select tags
- file input tags
- multiple inputs
- null values on controlled inputs

Each of these tags and techniques solve issues for common use cases for forms in react. 

## Brandon Moreli: Ternary Operators
This article is available [here](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

The ternary operator roughly functions as a substitute for an if...else statement. Moreli summarizes the use of the ternary operator with this code line:

`condition ? value if true : value if false`

This is the basic form, and can handle a basic conditional with two outcomes. But what if...

![we need to go... deeper](https://allisonmaruska.files.wordpress.com/2015/10/we-need-to-go-deeper.jpg)

...well then we can simply nest one ternary in another!

`condition ? (condition ? value if true : value if false) if true : value if false`

This looks like it could get messy quickly, but for simple multi-conditionals it can be useful shorthand. 

## Additional Bookmarks

[React Bootstrap: Forms](https://react-bootstrap.github.io/components/forms/)

[React Docs: Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)


[<<Return to Home](../README.md)