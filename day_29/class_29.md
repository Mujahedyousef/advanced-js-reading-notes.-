[Redux - Additional Topics Live Url](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_29/class_29.html)

## Redux Toolkit

* The Redux Toolkit package is intended to be the standard way to write Redux logic.

* It was originally created to help address three common concerns about Redux:

 1. Configuring a Redux store is too complicated
 1. I have to add a lot of packages to get Redux to do anything useful
 1. Redux requires too much boilerplate code

### Installation

* Redux Toolkit is available as a package on NPM for use with a module bundler or in a Node application:

```
npm install @reduxjs/toolkit
```

## Redux Toolkit includes these APIs

1. configureStore( ): wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.
1. createReducer( ): that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos[3].completed = true.
1. createAction(): generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.
1. createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.
1. createAsyncThunk:  accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise
1. createEntityAdapter:  generates a set of reusable reducers and selectors to manage normalized data in the store
1. The createSelector utility from the Reselect library, re-exported for ease of use.

* [more info](https://redux-toolkit.js.org/introduction/getting-started).

----

## MobX

* is a simple, scalable, and battle-tested state management solution.
* MobX is a standalone library.

* MobX makes state management simple again by addressing the root issue: it makes it impossible to produce an inconsistent state. The strategy to achieve that is simple: Make sure that everything that can be derived from the application state, will be derived. Automatically.

* [more info](https://mobx.js.org/getting-started.html).

----

## [Hookstate](https://hookstate.js.org/docs/getting-started)
