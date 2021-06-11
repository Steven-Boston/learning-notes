# Reading 301-5: Thinking in React
This document is available [here](https://reactjs.org/docs/thinking-in-react.html)

This reading is an overview of how to concept projects and ideas in the context of react.js design. The document offers a process for implementing a desired product in steps: 

1. Break The UI Into A Component Hierarchy
  * Make a "react wireframe" that is a visual breakdown of the task at hand by representing components as boxes. Each component should have one primary functionality. 
2. Build A Static Version in React
  * Code the app as designated in the wireframe with all of the structure but no interactivity.
3. Identify The Minimal (but complete) Representation Of UI State
  * Find the smallest number of data that can be stored in state and maintain the interactivity of your app in order to keep track of things like user inputs. 
4. Identify Where Your State Should Live
  * Locate the components at the highest point in the component hierarchy that need access to the state data and assign those state values to them.
5. Add Inverse Data Flow
  * Build the functionality your app needs to pass that state data from the inputs (probably on lower lebvel components) up to where the state lives. 




[<<Return to Home](README.md) 