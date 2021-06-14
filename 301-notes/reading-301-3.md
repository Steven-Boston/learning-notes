# REAding 301-3: Passing Functions as props

## React: Lists and Keys
This document is available [here](https://reactjs.org/docs/lists-and-keys.html)

This documentation discusses techniques to use with lists in react, namely how to convert them into elements and how to add a key attribute so that each element has a discernable identity. This is generally achieved by useing array.map to create a new array by modifying the list items, which should use the provided data and reform it into a React Element with corresponding attributes to be passed via props. 

## JavaScript: Using the Spread Operator
This document is available [here](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

The spread operator (`...`) is used to manipulate arrays. The effect is straightforward: The operation takes an array and breaks it into individual pieces to be used in ways an array cannot:
- being passed as multiple arguments in a function 
- being copied into a new array (rather than a reference to the original) `newArray = [...oldArray]`
- being broken into parts and added with another array (`bigArray = [...oldArray, ...olderArray]`)

Similar tactics give us the ability to reinitiate the array with new items, perhaps so that it can be updated in a state in React. 

## Video: How to Pass Functions Between Components
This Video is available [here](https://www.youtube.com/watch?v=c05OL7XbwXU)

This short video covers the techniques used to pass a function via props. The host has an increment function that is to be used by each of several child components to find and increment the counter corresponding to the child element's name. He is able to execute this by simply passing the function into a value of a key for the props. We can then access the function via its prop extension. 


[React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

[<<Return to Home](../README.md)