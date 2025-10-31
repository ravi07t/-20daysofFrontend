Today’s Focus:
1.	What is useRef() and what are its use cases?
useRef() is used to persist values, access DOM elements, and store mutable data without re-rendering the component. Used to directly manipulate DOM elements, like focusing an input field. The value stored in ref.current does not cause re-render when changed. It helps optimize performance by avoiding unnecessary re-renders when tracking values that don’t affect the UI.

2.	What is useMemo() and why is it used?
useMemo() does not prevent re-rendering, but it prevents re-computation of certain values. It helps optimize performance by preventing unnecessary recalculations of expensive operations during re-renders. useMemo() Hook in React is used to memoize (cache) the result of a computation so that it is recalculated only when its dependencies change.

3.	What is useCallback()
useCallback() Hook in React is used to memoize (cache) a function so that it is not recreated on every re-render, unless its dependencies change. It helps prevent unnecessary re-creations of functions and is mainly used to optimize performance when passing callbacks to child components.

4.	Difference between useMemo() and useCallback()?
useMemo() - Returns a memoized value. Memoizes (caches) the result of a computation and returns the value, used to avoid recalculating expensive values or computations unnecessarily. When you need to cache computed data (filtered lists, calculations).

useCallback() - Returns a memoized function. Memoizes (caches) a function definition and returns the function itself. Used to avoid recreating functions unnecessarily during re-renders. When you pass functions to memoized child components (React.memo) to prevent re-renders.

5.	Why, When to use React.memo()?
React.memo() is a higher-order component (HOC) that is used to optimize performance by preventing unnecessary re-renders of a functional component. When a parent component re-renders, all its child components also re-render even through children props haven’t changed. To avoid we use React.memo() in all components.
