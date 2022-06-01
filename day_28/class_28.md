[Redux - Asynchronous Action Live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_28/class_28.html)

## Redux - Asynchronous Action

* Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects.
* Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.
* There are two very popular middleware libraries that allow for side effects and asynchronous
actions:
  * Redux Thunk
  * Redux-Saga

### Redux Thunk

* Thunk is a programming concept where a function is used to delay the evaluation

## stages

1. First, use the terminal to navigate to the project directory and install the redux-thunk package

```
npm install redux-thunk@2.3.0
```

2. apply the middleware when creating your app’s store using Redux’s applyMiddleware. Given a React application with redux and react-redux, your index.js file

```
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from 'react-redux';
import { createStore, applyMiddleware } from 'redux';
import thunk from 'redux-thunk';
import './index.css';
import rootReducer from './reducers';
import App from './App';


// use applyMiddleware to add the thunk middleware to the store
const store = createStore(rootReducer, applyMiddleware(thunk));

ReactDOM.render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root')
);
```

3. The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.
