# REACT JS

## WHAT IS REACT JS?
- Created by Facebook, ReactJS is a JavaScript library designed for crafting dynamic and interactive applications, elevating UI/UX for web and mobile platforms. Operating as an open-source, component-based front-end library, React is dedicated to UI design and streamlines code debugging by employing a component-oriented approach.
### KEY FEATURES OF REACT JS
1. JSX(JavaScript Syntax Extension):

- JSX is a combination of HTML and JavaScript. You can embed JavaScript objects inside the HTML elements. JSX is not supported by the browsers, as a result, Babel compiler transcompile the code into JavaScript code. JSX makes codes easy and understandable. It is easy to learn if you know HTML and JavaScript.
<div style="display: flex;">

  <div style="flex: 50%; padding: 10px;">
    ## Column 1
    This is the content for the first column. You can add **text**, *images*, or other Markdown elements here.
  </div>
const name="GeekforGeeks";
const ele = <h1>Welcome to {name}</h1>;
  <div style="flex: 50%; padding: 10px;">
    ## Column 2
    This is the content for the second column. Similarly, add more **text**, *images*, etc.
  </div>

</div>

2. Declarative Programming:

- With React, developers describe how the UI should look at any given time based on the app's state. React then handles the updates efficiently, making the development process more intuitive and predictable.

3. Virtual DOM:

- React uses a Virtual DOM, which is a lightweight copy of the actual DOM. When a component's state changes, React first updates the Virtual DOM and then compares it with the real DOM. This reconciliation process minimizes the number of actual DOM manipulations, improving app performance.

4. Unidirectional Data Flow:

- React enforces one-way data binding, meaning data flows in a single direction, typically from parent components to child components. This makes it easier to understand how data changes and where the changes originate.

5. JSX (JavaScript XML):

- React employs JSX, a syntax extension that allows you to write HTML-like code within JavaScript. JSX makes it easier to create and visualize the structure of the UI alongside the logic for handling user interactions.
 
6. State and Props:

- State represents mutable data specific to a component, and React automatically re-renders the component when its state changes.
Props are immutable data passed from a parent component to a child. They enable communication between components and are read-only.

7. Hooks:

- Introduced in React 16.8, Hooks allow functional components to manage state and side effects without needing class-based components. Popular hooks include useState for state management and useEffect for handling side effects like data fetching or subscribing to external services.

8. Ecosystem and Tools:

- React has a rich set of accompanying tools and libraries, including React Router for managing navigation and Redux for centralized state management. There’s also React Native, which extends React’s principles to mobile app development.