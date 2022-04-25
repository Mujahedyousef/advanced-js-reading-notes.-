[Component Based UI Live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_17/class_17.html)

# Reading: Component Based UI

## React:

Is a JavaScript library, that enables us to create UIs using multiple reusable components.

---

## react hello world

```
.createRoot(document.getElementById('root'))
.render(<h1>Hello, world!</h1>);
```

---

## JSX

> and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like.

- comes with the full power of JavaScript.
- JSX produces React “elements”.

## Why JSX?

1. React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.
1. Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

1. JSX allows React to show more useful error and warning messages.

- **Features**

1. JSX allows us to write HTML in React.
1. JSX makes it easier to write and add HTML in React.

1. JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement() and/or appendChild() methods.
1. JSX converts HTML tags into react elements.
1. JSX is an extension of the JavaScript language based on ES6, and is translated into regular JavaScript at runtime.

---

## Rendering Elements

> An element describes what you want to see on the screen.

- Unlike browser DOM elements, React elements are plain objects and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

- Updating the Rendered Element (Links to an external site.)

React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time. With our knowledge so far, the only way to update the UI is to create a new element, and pass it to root.render().
