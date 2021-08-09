# Passing Functions as Props
## **Lists and Keys**:


we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

`const numbers = [1, 2, 3, 4, 5];`

`const doubled = numbers.map((number) => number * 2);`

`console.log(doubled);`

This code logs [2, 4, 6, 8, 10] to the console.

In React, transforming arrays into lists of elements is nearly identical

**Basic List Component**

Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

`function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>    <li>{number}</li>  );  return (
    <ul>{listItems}</ul>  );
}`

`const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,  document.getElementById('root')
);`

**Keys**

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

`const numbers = [1, 2, 3, 4, 5];`

`const listItems = numbers.map((number) =>`

  `<li key={number.toString()}>`
      `{number}</li> `

`);`

  



--------


**To know more please 
[visit this page](https://reactjs.org/docs/lists-and-keys.html)**

-------

-----------

## **The Spread Operator:**

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
Mounting, Updating, and Unmounting are Part of the component lifecycle.

What is `...` used for?

    “Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.” — JavaScript.info

Take trying to find the largest number in an array with `Math.max()`:

`Math.max(1,3,5)` // 5

`Math.max([1,3,5])` // NaN

`Math.max(...[1,3,5])` // 5

Also:
- **Copying an array**
- **Concatenating or combining arrays**
- **Using Math functions**
- **Using an array as arguments**
- **Adding an item to a list**
- **Adding to state in React**
- **Combining objects**
- **Converting NodeList to an array**
 
 EX:

 `[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]`

`[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]`


`const hello = {hello: "😋😛😜🤪😝"}`


`const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}`


`const helloWorld = {...hello,...world}`

`console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }`



--------


**To know more please 
[visit this page](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)**

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