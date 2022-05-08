- [useReducer() Hook live Url](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_20/class_20.html)

---

# useReducer ( )

- is one of the additional Hooks that shipped with React v16.8. An alternative to the useState Hook, useReducer helps you manage complex state logic in React applications.

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

```
 const initialState = {count: 0};

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return {count: state.count + 1};
    case 'decrement':
      return {count: state.count - 1};
    default:
      throw new Error();
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({type: 'decrement'})}>-</button>
      <button onClick={() => dispatch({type: 'increment'})}>+</button>
    </>
  );
}
```

## The reducer function


> The JavaScript reduce() method executes a reducer function on each element of the array and returns a single value. The reduce() method accepts a reducer function, which itself can accept up to four arguments.
-----
## The dispatch method


* The dispatch function accepts an object that represents the type of action we want to execute when it is called. Basically, it sends the type of action to the reducer function to perform its job, which, of course, is updating the state.

* The action to be executed is specified in our reducer function, which in turn, is passed to the useReducer. The reducer function will then return the updated state.

* The actions that will be dispatched by our components should always be represented as one object with the type and payload key, where type stands as the identifier of the dispatched action and payload is the piece of information that this action will add to the state.
----
[Read more](https://blog.logrocket.com/react-usereducer-hook-ultimate-guide/#specifying-initial-state)