Today’s Focus:
1.	What are React Hooks?
Hooks introduced in React 16.8 to make functional components more powerful and cleaner. Hooks are special functions in React that let you use state and other React features in functional components.
Commonly Used React Hooks:
	
useState	Adds state to functional components
useEffect	Handles side effects (e.g., data fetching, DOM updates)
useContext	Accesses values from Context API directly
useRef	Accesses or stores mutable values or DOM elements
useMemo	Memoizes expensive calculations
useCallback	Memoizes functions to prevent unnecessary re-renders
useReducer	Manages complex state logic (alternative to useState)
useLayoutEffect	Similar to useEffect but runs synchronously after all DOM mutations
useImperativeHande	Customizes instance values when using ref with forwardRef

2.	What is useState() in React?
useState() is a React Hook that lets you add state to functional components.
It allows a component to store data that can change over time and automatically re-render the component when that data changes.
React sets the state variable to the initial value When the component renders for the first time, when you call the setter function (setState), React Updates the state value and re-renders the component with the new state Each render gets its own snapshot of the state value.

3.	What is useEffect()?
useEffect() is a React Hook that allows you to perform side effects in functional components. useEffect is function we call thi function by passing another function to it which is called callback function.
Syntax:- useEffect(callback function, dependency);
useEffect will be called on every render, which is bad way. If we don’t want to call it after every render pass in a dependency array into it.
Syntax:- useEffect(() => {}, []);
So, useEffect will be called just once initial render and after initial render it doesn’t re-render because of dependency array.

4.	Lifecycle methods in useEffect() hook?
Before useEffect hook these side effects were handled using class lifecycle methods such as componentDidMount, componentDidUpdate, and componentWillUnmount.
Mounting stage - componentDidMount() runs only once after the first render.
Updating stage – componentDidUpdate() runs every time the specified dependency changes
Unmounting stage – componentWillUnmount() runs before the component is removed from the DOM (for cleanup) like removing event listeners or clearing timers.

5.	Difference between useEffect() and useLayoutEffect()?
useEffect() runs after the component has been rendered and painted to the screen. Runs asynchronously after the browser has finished painting the DOM. Does not block the browser from updating the UI.

useLayoutEffect() runs synchronously after DOM updates but before the browser paints the screen. Runs immediately after React updates the DOM, but before the user sees the changes. It can block the browser’s paint, so it is used only for critical DOM operations.
