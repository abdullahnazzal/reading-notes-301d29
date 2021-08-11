# PassReadings: React and Forms
## **Forms**:

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:

`<form>`

  `<label>`
  
  `Name:`
    `<input type="text" name="name" />`

  `</label>`

  `<input type="submit" value="Submit" />`

`</form>`



**Controlled Components**



In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

**Keys**

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

`const numbers = [1, 2, 3, 4, 5];`

`const listItems = numbers.map((number) =>`

  `<li key={number.toString()}>`
      `{number}</li> `

`);`

  



--------


**To know more please 
[visit this page](https://reactjs.org/docs/forms.html)**

-------


## **The Conditional (Ternary) Operator Explained:**

The ternary operator:


`condition ? value if true : value if false`


Here’s what you need to know:

1- The `condition` is what you’re actually testing. The result of your condition should be `true` or `false` or at least coerce to either boolean value.

2- A `?` separates our conditional from our true value. Anything between the `?` and the `:` is what is executed if the `condition` evaluates to true.

3- Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

**Example — Driver Age**

We’ll take a moment to revisit the initial example in this article:

`let person = {`

  `name: 'tony',`

  `age: 20,`

  `driver: null`

`};`

`person.driver = person.age >=16 ? 'Yes' : 'No';`


--------


**To know more please 
[visit this page](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)**

-------

## **Passing Functions to Components**


**In the video, what is the first step that the developer does to pass functions between components?**

Wherever the state going to change.

**In your own words, what does the increment function do?**

Update when you Click on.

**How can you pass a method from a parent component into a child component?**

By using props

**How does the child component invoke a method that was passed to it from a parent component?**

By passing attribute to the compoent.

--------


**To know more please 
[visit this Video](https://www.youtube.com/watch?v=c05OL7XbwXU)**

-------