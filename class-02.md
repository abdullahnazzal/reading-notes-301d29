# State and Props
## **lifecycle**:

### **What are component lifecycle events?**

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states
<br>

![What are component lifecycle events](img/LS.png)



Mounting, Updating, and Unmounting are Part of the component lifecycle.

- **Mounting**:
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

- **Updating**:
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.

- **Unmounting**:
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

**- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

render will run first.

**- What is the very first thing to happen in the lifecycle of React?**
constructor()

**- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**

1- constructor.
2- render.
3- componentDidMount.
4- React Updates.
5- componentWillUnmount.

**- What does componentDidMount do?**

to load anything using a network request or initialize the DOM.

--------


**To know more please 
[visit this page](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)**

-------

### **React State Vs Props?**

<br>

1- What types of things can you pass in the props?

Any things from number to object.

2- What is the big difference between props and state?

state is handled in the component and you can update it inside the component.

props are handled outside the component and must be updated outside of the component.

3- When do we re-render our application?

when we change something in the app.

4- What are some examples of things that we could store in state?

any type of data.

--------


**To know more please 
[visit this Video](https://www.youtube.com/watch?v=IYvD9oBCuJI)**

-------