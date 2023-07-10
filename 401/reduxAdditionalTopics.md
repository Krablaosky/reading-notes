## Redux - Additional Topics

### Reading

#### [Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)

1. Redux Toolkit (RTK) addresses several concerns in Redux development, including:
   - Simplifying the Redux development workflow by providing a set of opinionated helpers and utilities.
   - Encouraging best practices for writing Redux code, such as using immutable updates and structured code organization.
   - Reducing boilerplate code by abstracting away common tasks like creating actions, reducers, and store configuration.
   - Improving performance through optimized reducer logic and memoized selectors.
   - Providing a standardized way of defining Redux state and actions using the "slice" concept.

2. The `configureStore()` function in Redux Toolkit is used to create a Redux store with sensible defaults and middleware pre-configured. It combines several Redux core functions and third-party middleware, such as Redux Thunk, into a single convenient setup. `configureStore()` automatically sets up the Redux DevTools extension for debugging and enables additional features like immutable state usage checks.

3. The `createSlice()` function is used to define a "slice" of Redux state, which includes the corresponding reducer logic and action creators. It generates the reducer function and action creators based on the provided configuration object. The `createSlice()` function reduces the boilerplate code required to set up actions and reducers manually. It automatically generates action types and action creators based on the names of the reducer functions defined within the slice.

#### [MobX](https://mobx.js.org/getting-started.html)

1. MobX is a state management library for JavaScript applications. It allows you to create observable state and automatically tracks the dependencies between state values and computed properties. MobX follows the reactive programming paradigm, where changes in the state automatically propagate to the affected parts of the application, keeping the user interface in sync with the data.

2. MobX makes it "impossible" to produce an inconsistent state by enforcing strict rules for modifying the state. In MobX, you should only modify the state within "actions." Actions are functions that modify the state and are decorated with the `@action` decorator or created using the `action()` function. By ensuring that state modifications only occur within actions, MobX guarantees that the state transitions are predictable and avoids potential inconsistencies.

3. To build a reactive user interface with MobX, you need to define observable state and computed properties. Observable state refers to the data that is tracked for changes, while computed properties are derived values that depend on the observable state. When the observable state changes, MobX automatically updates the computed properties and triggers re-evaluation of any reactive components that depend on them. Reactive components can be implemented using frameworks like React, Angular, or Vue, which have integration libraries for MobX.

### Tutorial

#### [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

1. The tutorial provides the following takeaways:

   - Redux Toolkit tutorials on the Redux core documentation site provide comprehensive guidance for learning Redux and using Redux Toolkit with React-Redux.
   - The Redux Toolkit Quick Start tutorial introduces adding and using Redux Toolkit in a React application.
   - The Redux Essentials tutorial teaches Redux concepts and best practices using Redux Toolkit for writing Redux logic.
   - The Redux Fundamentals tutorial explains how Redux works, shows manual Redux code, and demonstrates how Redux Toolkit simplifies usage patterns.

## [Back](../401readingNotes.md)