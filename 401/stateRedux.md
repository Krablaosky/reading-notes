# Application State with Redux

## Reading

### [Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

1. **What is the first principle of Redux?**
   
   The first principle of Redux is that the whole application state is stored in a single JavaScript object called the "state tree" or "store". This allows the state to be managed and updated in a predictable and centralized manner.

2. **What is a store and what do we use our reducers for within that store?**
   
   A store in Redux is an object that holds the application state and provides methods to interact with it. It is the central hub of Redux, responsible for dispatching actions and triggering state updates. Reducers are used within the store to specify how the application state should change in response to different actions.

3. **Name three Redux store methods given to us by createStore and describe their use.**
   
   - `getState()`: This method is used to retrieve the current state of the application from the store.
   - `dispatch(action)`: It is used to dispatch an action, triggering the corresponding state update based on the logic defined in the reducers.
   - `subscribe(listener)`: This method allows you to register a listener function that will be called whenever the state in the store changes. It is commonly used to update the user interface when the state updates.

4. **Explain to a non-technical recruiter what combineReducers() does and why it is useful.**
   
   `combineReducers()` is a utility function provided by Redux that allows you to combine multiple reducers into a single reducer function. It is useful because as an application grows, the number of reducers can increase, and managing them individually can become complex. `combineReducers()` simplifies this process by merging multiple reducers into one, creating a single root reducer that can be used in the store. This helps organize the application state and makes it easier to maintain and reason about the state management in Redux.

## Bookmark and Review

- [World's Easiest Guide to Redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

- [Testing Reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

- [Redux Docs](https://redux.js.org/)
