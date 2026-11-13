# Exp 9 – React Lab Exercise: React Fragments
## NAME: Paladugu Venkata Balaji
## REG NO: 2305001024
## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
Understand the concept of React Fragments.
Use Fragment shorthand syntax.
Use the explicit Fragment syntax.
Group multiple JSX elements without an extra DOM node.
Understand the difference between Fragments and div elements.
# Program
## Step 1: Create a React Project
~~~
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
~~~
Select React as the framework and JavaScript as the variant.

## Step 2: App.jsx – Using Fragment Shorthand
~~~
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name:Paladugu Venkata Balaji</h3>

      <p>Register Number: 2305001024</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
~~~
## Step 3: Using Explicit Fragment Syntax
~~~python
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name:Paladugu Venkata Balaji</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
~~~
## Output
## Fragment Shorthand Syntax
<img width="1358" height="655" alt="image" src="https://github.com/user-attachments/assets/158ad81d-d0dc-4c86-8052-e9fbc366b5fc" />


## Explicit Fragment Syntax
<img width="1671" height="682" alt="image" src="https://github.com/user-attachments/assets/a7dc68b4-5b6f-4599-8a70-813a00943e38" />


## Result
Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
