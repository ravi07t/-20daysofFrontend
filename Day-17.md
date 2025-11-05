Today’s Focus:

1.	What is prop drilling?
Prop drilling is the process of passing data from a parent component down to deeply nested child components through multiple levels of props even when some intermediate components don’t need that data.

2.	What is contextAPI?
To avoid prop drilling in React, we use Context API, state management libraries (like Redux). The Context API lets you share data across components without passing props manually at every level.
1.	createContext() – Used to create a context object.
2.	Provider – Used to wrap components and provide the data (state or value).
3.	useContext() – Used inside child components to consume or access the provided data.

3.	What is Redux and why do we use it?
Redux as a centralized data store for your entire app. Instead of passing data between multiple components manually (via props), Redux stores all the data in one place (the store), and components can access or update it easily.
•	Single Source of Truth - The entire application state is stored in one central store.
•	State is Read-Only - The only way to change the state is to dispatch an action.
•	Changes are made with Pure Functions - Reducers are pure functions that take the previous state and action, and return the new state.

4.	What is an Action, Reducer, and Store in Redux?
Action: An object that describes what to do.
Example: { type: "INCREMENT", payload: 1 }

Reducer: A pure function that takes state and action as input and returns the new state.
Example: function counterReducer(state = 0, action) {
  if (action.type === "INCREMENT") return state + 1;
  return state;
}

Store: The single object that holds the application state and provides methods like getState(), dispatch(), and subscribe().

5.	What is useSelector() and useDispatch()?
useSelector(): A React hook used to access data from the Redux store.
Example: const count = useSelector((state) => state.counter.value);

useDispatch(): A React hook used to dispatch actions to the store.
Example: const dispatch = useDispatch();
dispatch(increment());
