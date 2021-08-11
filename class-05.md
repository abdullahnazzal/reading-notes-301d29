# Readings: Putting it all together
## **Thinking in React**:

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.



**How would you break a mock into a component heirarchy?**

Step 1: Break The UI Into A Component Hierarchy 
Step 2: Build A Static Version in React 
Step 3: Identify The Minimal (but complete) Representation Of UI State 
Step 4: Identify Where Your State Should Live 
Step 5: Add Inverse Data Flow 

**What is the single responsibility principle and how does it apply to components?**

ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

**What does it mean to build a ‘static’ version of your application?**

This is the easiest way is to build a version that takes your data model and renders the UI but has no interactivity.

**Once you have a static application, what do you need to add?**

I need to build components that reuse other components and pass data using props. 

**What are the three questions you can ask to determine if something is state?**


1- Is it passed in from a parent via props? If so, it probably isn’t state.

2- Does it remain unchanged over time? If so, it probably isn’t state.

3- Can you compute it based on any other state or props in your component? If so, it isn’t state.





**How can you identify where state needs to live?**

For each piece of state in your application:

- Identify every component that renders something based on that state.

- Find a common owner component (a single component above all the components that need the state in the hierarchy).

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

--------


**To know more please 
[visit this page](https://reactjs.org/docs/thinking-in-react.html)**

-------
