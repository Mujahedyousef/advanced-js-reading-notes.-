[Redux - Combined Reducers Live Url](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_27/class_27.html)

## Redux - Combined Reducers

* ## Core Concepts

>The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

* Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

> Important ideas to be aware of when using combineReducers:

* First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario. It is entirely possible to write reducer logic without using it, and it is quite common to need to write custom reducer logic for cases that combineReducer does not handle.
* While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors.

* combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.
* You can use it at all levels of your reducer structure, not just to create the root reducer. It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer.

* ## Defining State Shape

> There are two ways to define the initial shape and contents of your store's state.

1. First, the **createStore** function can take **preloadedState** as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser's localStorage.
2. The other way is for the root reducer to return the initial state value when the state argument is undefined. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using **combineReducers**.

* combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object. The correlation between these names is not always apparent, especially when using ES6 features such as default module exports and object literal shorthands.

----
[Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

[Combined Reducer Syntax]( https://redux.js.org/api/combinereducers/)
