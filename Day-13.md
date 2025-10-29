Today’s Focus:
1.	Virtual DOM in React?
The Virtual DOM (VDOM) is a lightweight copy of the Real DOM that React uses to improve the performance of web applications. It is a JavaScript object that represents the structure of the UI in memory. When a React application starts, the Virtual DOM is created from the React components. When a component’s state or props change, React creates a new Virtual DOM tree that reflects the updated UI. React compares the new Virtual DOM with the previous one using an efficient diffing algorithm. Only the elements that changed are updated in the real DOM.

2.	What is reconciliation?
This process of updating the real DOM based on changes in the Virtual DOM is called reconciliation.

3.	What is the purpose of key prop in lists?
The key prop is a special attribute each element in a list should have a unique key so that React can keep track of each item React identify which items have changed, been added, or removed in a list.

4.	What are controlled and uncontrolled components?
Controlled Components: A controlled component is a form element whose value is controlled by React state. Any change in input updates the state using an event handler.

Uncontrolled Components: An uncontrolled component is a form element that manages its own state internally in the DOM, React does not control the value directly. React does not control the value directly.

5.	How to lift state up between components?
Lifting state up means moving shared state to a common parent component so that multiple child components can access and modify the same data using props. To share data between multiple components.
