# Reading 301-1: React & Components

## Tutorialspoint: Component-Based Architecture
This article can be found [here](tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

A component is a singular item of software intended to work in tandem with other components. A component can be used repeatedly as necessary and has its own defined purpose and presentation. There are three different forms in which a component can be created, known as 'views':

#### Object-Oriented View:

The component is a framework of classes that both define and explain its functionality. The interface in which the classes are active must also be defined. 

#### Conventional View:

I read the folliwing paragraph several times and found it inscrutable: 

> "It is viewed as a functional element or a module of a program that integrates the processing logic, the internal data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data to be passed to it."

#### Process-Related View:

The component(s) are created via building blocks predefined in a library, and coordinated to behave in a certain way. 

### The Purpose of Components Based Design

Designing with components has many advantages: It can provide separation of concerns at a more granular level, improve efficiency both in execution and design, and make working on a large project more approachable and easier to prosecute for multiple developers. Individual fragments of the design can be used an reused at need, and mapping out the overall project implementation becomes more streamlined. 


## Cem Eygi on React: Props
This article can be found [here](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

Props is a keyword that is used in React.js, and is short for 'properties.' Props are used to facilitate the passing of data from disparate React components. This data flows from parent to child, and is read-only. 

`<ChildComponent attribute={'myData'}>` lets us set an attribute to the child component, 

then, giving props to a component function lets us pass it `const ChildComponent = props => <p>Here is my data</p>`. Now the object props will have a property matching the one we assigned to ChildComponent. From there we can access props.attribute from the child to get the value of the attribute. 


## Additional Bookmarks

[React Tutorial: Passing Data Through Props](https://reactjs.org/tutorial/tutorial.html)
[React Docs: Hello World](https://reactjs.org/docs/hello-world.html)
[React Docs: Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
[React Docs: Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
[React DocsL Components and Props](https://reactjs.org/docs/components-and-props.html)

[<<Return to Home](README.md) 