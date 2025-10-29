Today’s Focus:
1.	What are higher-order components (HOC)?
Higher-Order Component (HOC) is a function that takes a component as input and returns a new enhanced component. It’s used to reuse logic between multiple components without repeating code. A function that adds extra power to your component that is HOC.

2.	How do you pass data from child to parent?
This is done using callback functions.

3.	What is prop drilling and how can it be avoided?
Prop drilling is the process of passing data from a parent component down to deeply nested child components through multiple layers of intermediate components that don’t actually need the data. Avoid it using Context API.

4.	What is Context API and how does it work?
To share data (state, functions, or values) across multiple components without having to pass props manually at every level, it helps to avoid prop drilling. Context API is mainly used when certain data needs to be accessible by many components.

5.	What are Pure Components?
Pure Component is a component that re-renders only when its props or state change. It helps improve performance by preventing unnecessary re-renders. Normally, when a parent component updates, all its child components re-render even if their data hasn’t changed. In functional components, we use React.memo() to achieve the same behavior.
