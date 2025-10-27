
Today’s Focus:
3.	What is Reactjs? What are the main features of React?
React is open-source JavaScript library for creating interactive user interface using components, that is used for building UI especially for single page application. The main features of react it’s efficient, flexible, JSX, Virtual DOM, React Hooks, one-way data binding, creative custom components, developed tools and it’s easy to use. It was created by Facebook, today all tech companies are used to handle all web apps and mobile devices.

4.	What is JSX and Can browsers read JSX directly?
JavaScript Syntax Extension JSX is a JavaScriptXML, it is a extension to the JavaScript. JSX is combination of JavaScript, HTML, custom tags, CSS styles these technologies are written in single function it is called JSX, it will make react more elegant and simpler. Basically, browser doesn’t understand directly, browser only understand HTML, JavaScript. So, react uses transpilers like babel these transpilers convert JSX code to browser understandable language. 

5.	What are components in React?
React primarily uses two types of components
Function Components: These are simple JavaScript functions that accept props as an argument and return React elements. They are generally preferred for their simplicity and are commonly used with React Hooks for managing state and lifecycle effects.
    function Welcome(props) {
      return <h1>Hello, {props.name}</h1>;
    }
Class Components: These are ES6 classes that extend React.Component and include a render() method that returns React elements. Class components were traditionally used for managing state and lifecycle methods but are less common in modern React development due to the rise of Hooks.
    class Welcome extends React.Component {
      render() {
        return <h1>Hello, {this.props.name}</h1>;
      }
    }

6.	What are props in React?
Props are data transfer from one component to another component. Props are the primary way to transfer data component tree, from a parent component to its direct children unidirectional data flow, meaning data flows from top to bottom. Props are immutable once a component receives props, it should not modify them.

7.	What is state in React?
State is private to the component that owns it and is not directly accessible by other components, its behavior rendering dynamic updates to the UI. States are mutable value can be update should done by using setState.

