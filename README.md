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

### STEP BY STEP HOW TO SET UP REACT JS

# Installing ReactJS using webpack and babel

- Webpack is a module bundler (manages and loads independent modules). It takes dependent modules and compiles them to a single (file) bundle. You can use this bundle while developing apps using command line or, by configuring it using webpack.config file.

- Babel is a JavaScript compiler and transpiler. It is used to convert one source code to other. Using this you will be able to use the new ES6 features in your code where, babel converts it into plain old ES5 which can be run on all browsers.

# Step 1 - Create the Root Folder
- ## Create a folder with name reactApp on the desktop to install all the required files, using the mkdir command.

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
   C:\Users\username\Desktop>mkdir reactApp
   C:\Users\username\Desktop>cd reactApp

</div>

- To create any module, it is required to generate the package.json file. Therefore, after Creating the folder, we need to create a package.json file. To do so you need to run the npm init command from the command prompt.

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    C:\Users\username\Desktop\reactApp>npm init

</div>

- This command asks information about the module such as packagename, description, author etc. you can skip these using the –y option.

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    ## Command

    ```bash
    C:\Users\username\Desktop\reactApp>npm init -y
    ```
  </div>

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc;">
    ## Output

    ```json
    Wrote to C:\reactApp\package.json:
    {
       "name": "reactApp",
       "version": "1.0.0",
       "description": "",
       "main": "index.js",
       "scripts": {
          "test": "echo \"Error: no test specified\" && exit 1"
       },
       "keywords": [],
       "author": "",
       "license": "ISC"
    }
    ```
  </div>

</div>

# Step 2 - install React and react dom
- Since our main task is to install ReactJS, install it, and its dom packages, using install react and react-dom commands of npm respectively. You can add the packages we install, to package.json file using the --save option.

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    C:\Users\Tutorialspoint\Desktop\reactApp>npm install react --save
C:\Users\Tutorialspoint\Desktop\reactApp>npm install react-dom --save

</div>

Or, you can install all of them in single command as −

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
  C:\Users\username\Desktop\reactApp>npm install react react-dom --save

</div>

# Step 3 - Install webpack
- Since we are using webpack to generate bundler install webpack, webpack-dev-server and webpack-cli.

<div style="display: flex; justify-content: space-between;">

  <div style="flex: 1; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    C:\Users\username\Desktop\reactApp> npm install webpack --save
  </div>
  
  <div style="flex: 1; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    C:\Users\username\Desktop\reactApp> npm install webpack-dev-server --save
  </div>
  
  <div style="flex: 1; padding: 10px; border: 2px solid #ccc;">
    C:\Users\username\Desktop\reactApp> npm install webpack-cli --save
  </div>

</div>


Or, you can install all of them in single command as −


<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
  C:\Users\username\Desktop\reactApp>npm install webpack webpack-dev-server webpack-cli --save


</div>

# Step 4 - Install babel
- Install babel, and its plugins babel-core, babel-loader, babel-preset-env, babel-preset-react and, html-webpack-plugin

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
    const name = "GeekforGeeks";
    const ele = <h1>Welcome to {name}</h1>;

</div>

# Step 5 - Create the Files
- To complete the installation, we need to create certain files namely, index.html, App.js, main.js, webpack.config.js and, .babelrc. You can create these files manually or, using command prompt.

<div style="display: flex;">

  <div style="flex: 50%; padding: 10px; border: 2px solid #ccc; margin-right: 10px;">
    
   C:\Users\username\Desktop\reactApp>type nul > index.html
C:\Users\username\Desktop\reactApp>type nul > App.js
C:\Users\username\Desktop\reactApp>type nul > main.js
C:\Users\username\Desktop\reactApp>type nul > webpack.config.js
C:\Users\username\Desktop\reactApp>type nul > .babelrc

</div>

# Step 6 - Set Compiler, Server and Loaders
- Open webpack-config.js file and add the following code. We are setting webpack entry point to be main.js. Output path is the place where bundled app will be served. We are also setting the development server to 8001 port. You can choose any port you want.

webpack.config.js

const path = require('path');
const HtmlWebpackPlugin = require('html-webpack-plugin');

module.exports = {
   entry: './main.js',  // Entry file for the application
   output: {
      path: path.join(__dirname, '/dist'),  // Output directory (fixed from '/bundle' to '/dist')
      filename: 'bundle.js'  // Name of the output bundled JavaScript file
   },
   devServer: {
      inline: true,  // Enable inline mode for the development server
      port: 8001,  // Port to run the dev server on
   },
   module: {
      rules: [
         {
            test: /\.jsx?$/,  // Regex for JavaScript and JSX files
            exclude: /node_modules/,  // Exclude node_modules folder
            loader: 'babel-loader',  // Use Babel to transpile JS/JSX
            options: {
               presets: ['@babel/preset-env', '@babel/preset-react'],  // Updated Babel presets
            }
         }
      ]
   },
   plugins: [
      new HtmlWebpackPlugin({
         template: './index.html',  // Use index.html as a template for the output
      })
   ]
}