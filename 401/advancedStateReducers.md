# Advanced State with Reducers

## Reading

### [Extracting State Logic into a Reducer](https://react.dev/learn/extracting-state-logic-into-a-reducer)

1. What is the motivation for adding a reducer?
   * The motivation for adding a reducer is to manage complex state logic in a more organized and scalable manner. As an application grows, the state management needs can become more intricate, involving multiple related state variables and complex state transitions. A reducer helps centralize the state logic by providing a predictable way to update and manage state based on different actions. It promotes separation of concerns by separating state management from the component rendering logic.

2. What are actions in the context of a reducer? How are they different than setting state directly?
   * In the context of a reducer, actions are plain JavaScript objects that describe the type of state change or update that needs to be performed. Actions typically have a `type` property that represents the type of action being performed. They can also include additional data or payload that provides information necessary for the state update. Actions are different from directly setting state in that they serve as explicit instructions for the reducer to perform a specific state transition. Instead of directly mutating or updating the state, components dispatch actions to the reducer, which then handles the state update based on the action type.

3. What common list operation is useReduce named for, and why?
   * `useReducer` is named after the common list operation "reduce," which is also known as "fold" or "accumulate." The `reduce` operation takes a collection of values and combines them into a single value by applying a specified operation or function iteratively. Similarly, in the context of `useReducer`, the reducer function takes the current state and an action, and returns the new state by applying the specified logic or transformation. The reducer iteratively accumulates state updates based on dispatched actions, allowing complex state management to be handled in a more concise and predictable manner.

4. When should you switch from useState to useReducer?
   * You should consider switching from `useState` to `useReducer` when the state management in your component becomes more complex and involves multiple related state variables or complex state transitions. `useReducer` is especially useful when the state updates are based on a predefined set of actions and require more advanced logic. It provides a more scalable approach to state management by centralizing the state logic in a reducer function. Additionally, if you find that your component's state management is becoming difficult to maintain or reason about with `useState`, switching to `useReducer` can help organize and simplify the state management code.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

[useReducer hook](https://react.dev/reference/react/useReducer)

[Keeping Components Pure](https://react.dev/learn/keeping-components-pure)

[Queueing a Series of State Updates](https://react.dev/learn/queueing-a-series-of-state-updates)

## [Back](../401readingNotes.md)