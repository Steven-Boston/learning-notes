# Reading 201-6: Problem Domain, Objects, and the DOM

## John Sonmez: The Problem Domain
This article can be found [here](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

Sonmez has a short but valuable article here about the importance and difficulty of understanding the problem domain when approaching coding tasks. He describes a couple of examples that illustrate a simple fact: spending time mapping out the problem you are trying to solve makes coding the solution easier by several orders of magnitude.  

## Duckett JS 3 pp.100-105: Object Literals 

Objects model some sort of noun to manipulated via sets of variables (known as properties of the object) and functions (methods of the object). You can establish one with:
```
var bowHouse = {
  owner: 'Starkovich',
  rooms: 5,
  greetOwner: function() {
    return 'Hello ' + this.owner + ' family!';
  }
};
```
and then access the information later:
```
var bowRooms = bowHouse.rooms;
var greeting = bowHouse.greetowner;
```
or 
```
var bowRooms = bowHouse['rooms'];
var greeting = bowHouse['greetowner'];
```

## Duckett JS 5: Document Object Model

The dom is a guide for the browser that specifies the way a page should be displayed, and how alterations to the page made by javascript should be accepted and implemented. 

Browsers interpret html files as a tree with nodes for each element and their attributes, as well as the text within those elements. Broadly, the DOM tree can be manipulated in 2 steps. Those steps as outlined by Duckett are:
1. Access the elements
2. Work with those elements

within those steps are a number of strategies for executing them:

Access:
- `querySelector('CSS selector')`
- `getElementById('id')`
- `getElementsByClassName('class')`
- `getElementsByTagName()`
- `querySelectorAll('CSS selector')`

Traversal:
- `parentNode`
- `previousSibling/nextSibling`
- `firstChild/lastChild`

Work:
- `nodeValue` accesses the contents of text nodes, and is able to change them. 
- `innerHTML` works with content in the element and the child elements
- `textContent` will only affect the text of the element
- `createElement()` create a new element node
- `createTextNode()` create a new text node
- `appendChild()/removeChild()` 
- `className/Id` update those values
- `hasAttribute` verify presence of attribute
- `getAttribute` confirm the value of an attribute
- `setAttribute` Assign a new value to the attribute
- `removeAttribute` remove the attribute entirely

The location of a particular node in the DOM, once accessed, can (and should) be stored as a variable if it will be needed later to conserve browser processing time. Finding multiple nodes returns them as a nodeList: an array with values for each node route found. From there you can either pick nodes individually or loop through them all. nodeLists come with a method called `item('index')` that returns a particular node for use, but simply array index format is usually more efficient. From an alrady acquired node, the traversal properties can be used to quickly travel closeby. 

Once you are satisfied you have located the correct element, it is probably your intention to alter or use it in some fashion. If working on a text node, nodeValue gives you an avenue to manipulate it. Keep in mind that the text cannot be used from the container, but the text node itself. To change the text, we can store the nodeValue of the text node to a variable, then change the text within that variable, then re-store it in the node using the `element.nodeValue = textVariable`.

The chapter outlines adding and removing HTML content as well as the properties used to manipulate the DOM directly in detail that is too broad to cover in these notes. The chapter then finishes by discussing common security issues presented by manipulating HTML, and how scripts from malicious code can threated your site as well as your (or your users') data. 

[<<Return to Home](../README.md)