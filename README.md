# REACT JS

## WHAT IS REACT JS?
- Created by Facebook, ReactJS is a JavaScript library designed for crafting dynamic and interactive applications, elevating UI/UX for web and mobile platforms. Operating as an open-source, component-based front-end library, React is dedicated to UI design and streamlines code debugging by employing a component-oriented approach.
### KEY FEATURES OF REACT JS
1. JSX(JavaScript Syntax Extension):

- JSX is a combination of HTML and JavaScript. You can embed JavaScript objects inside the HTML elements. JSX is not supported by the browsers, as a result, Babel compiler transcompile the code into JavaScript code. JSX makes codes easy and understandable. It is easy to learn if you know HTML and JavaScript.
<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    const name = "GeekforGeeks";
    const ele = <h1>Welcome to {name}</h1>;

</div>

2. Virtual DOM:

- DOM stands for Document Object Model. It is the most important part of the web as it divides into modules and executes the code. Usually, JavaScript Frameworks updates the whole DOM at once, which makes the web application slow. But react uses virtual DOM which is an exact copy of real DOM. Whenever there is a modification in the web application, the whole virtual DOM is updated first and finds the difference between real DOM and Virtual DOM.

3. One-way Data Binding:

- One-way data binding, the name itself says that it is a one-direction flow. The data in react flows only in one direction i.e. the data is transferred from top to bottom i.e. from parent components to child components. The properties(props) in the child component cannot return the data to its parent component but it can have communication with the parent components to modify the states according to the provided inputs.

4. Performance:

- As we discussed earlier, react uses virtual DOM and updates only the modified parts. So , this makes the DOM to run faster. DOM executes in memory so we can create separate components which makes the DOM run faster.

5. Extension:

- React has many extensions that we can use to create full-fledged UI applications. It supports mobile app development and provides server-side rendering. React is extended with Flux, Redux, React Native, etc. which helps us to create good-looking UI.
 
6. Conditional Statements:

- JSX allows us to write conditional statements. The data in the browser is displayed according to the conditions provided inside the JSX.

### Syntax:
<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    const age = 12;
if (age >= 10)
{ 
    <p> Greater than { age } </p>;
} 
else 
{ 
    <p> { age } </p>;
}


</div>

7. Components:

- React.js divides the web page into multiple components as it is component-based. Each component is a part of the UI design which has its own logic and design as shown in the below image. So the component logic which is written in JavaScript makes it easy and run faster and can be reusable.

8. Simplicity:

- React.js is a component-based which makes the code reusable and React.js uses JSX which is a combination of HTML and JavaScript. This makes code easy to understand and easy to debug and has less code.
## Steps to Create React Application:
### Step 1: Create a react application by using the following command:
<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
npx create-react-app foldername

</div>

### Step 2: Change your directory to the newly created folder.
<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    cd foldername

</div>
