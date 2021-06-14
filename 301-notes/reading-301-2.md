# Reading 301-2: React: States and Props

## React: Component Lifecycle events
This article by Joshua Blankenship can be found [here](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

Components have a predictable lifestyle that comes in three phases. There are many different events that can occur along this timeline, and Blankenship's article has a full breakdown with a flowchart of each method:

- Mounting: Instance is created and appended to the DOM 
  * constructor
  * static getDerivedStateFromProps
  * render
  * componentDidMount
  * UNSAFE_componentWillMount

- Updating: Whenever a component is altered and the reinstantiated. 
  * static getDerivedStateFromProps
  * shouldComponentUpdate
  * render
  * getSnapshotBeforeUpdate
  * componentDidUpdate
  * UNSAFE_componentWillUpdate
  * UNSAFE_componentWillReceiveProps

- Unmounting: During the process of removing the component.
  * componentWillUnmount

Blankenship then walks through each of these methods and discusses the use cases and applications of each. He ends the article with a helpful quick reference chart, which I have included below for reference: 

![Component Method Chart](https://miro.medium.com/max/933/1*4y9V5936WdJKaIeVPFEa3w.png)



## Video: React: State vs. Props
This video from Web Dev Simplified can be found [here](https://www.youtube.com/watch?v=IYvD9oBCuJI)

The above video provides a brief breakdown of the delineation of props and state when it comes to handling data in React. The author points out that props is used to handle data provided from the parent component. This is to say that the props are used to initialize the component with certain prearranged values. Those values then become the starting state of the live component. The state then acts as the live storage for data for the component, and can change as the user interacts with it. As the state changes, the component can update its appearance or behavior appropriately. 

## Additional Bookmarks:

- [React Bootstrap Documentation](https://react-bootstrap.github.io/)
- [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
- [React Docs - handling events](https://reactjs.org/docs/handling-events.html)
- [React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)


[<<Return to Home](../README.md)