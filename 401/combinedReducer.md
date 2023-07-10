# Redux - Combined Reducers

## Reading

### [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

1. **Why create multiple reducers?**

   Multiple reducers are created in Redux to handle different slices of the application state. By splitting the state management into smaller, focused reducers, it becomes easier to understand, maintain, and update the state as the application grows in complexity. Each reducer can handle a specific part of the state and the corresponding actions, improving modularity and separation of concerns.

2. **How would you combine multiple reducers?**

   To combine multiple reducers in Redux, you can use the `combineReducers` function provided by Redux. This function takes an object where each key represents a slice of the state and the value represents the corresponding reducer function. The resulting combined reducer can be passed to the Redux store.

3. **How will you manage state as an immutable object? Why?**

   In Redux, it is recommended to manage state as an immutable object. This means that the state should not be directly mutated, but instead, a new state object should be created with the desired changes. Immutable state helps in maintaining a predictable state flow and enables efficient change detection, as it allows for easy comparison of state objects. It also helps with debugging and tracking state changes over time.

### [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

1. **`combineReducers` is a utility function to simplify the most common use case when writing ___ _____.**

   `combineReducers` is a utility function to simplify the most common use case when writing Redux reducers.

2. **Explain how `combineReducers` assembles the new state tree.**

   `combineReducers` assembles the new state tree by creating a new object where each key corresponds to a slice of the state, and the value is the result of calling the corresponding reducer function on that slice of the state. It merges the individual slice states returned by the reducers into a single state tree.

3. **How would you define initial state in an app using `combineReducers`?**

   When using `combineReducers`, you can define the initial state for each individual reducer by assigning it as the default value of the corresponding reducer function. Alternatively, you can use the `initialState` argument provided to each reducer when creating the combined reducer.

### [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

1. **Why will you want to split your reducing functions as your app becomes more complex?**

   As an app becomes more complex, splitting the reducing functions into smaller, focused reducers becomes important for better code organization and maintainability. It allows different parts of the state to be managed independently, making it easier to reason about the state changes and debug issues. It also facilitates code reuse and modularity, as reducers can be combined or reused in different parts of the application.

2. **The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.**

   The `combineReducers` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `Redux`.

3. **What is a popular convention when naming reducers?**

   A popular convention when naming reducers is to use the domain or slice of the state they manage as part of their names. For example, if a reducer manages the state related to user authentication, it could be named `authReducer`. This convention helps to clearly indicate the responsibility and scope of each reducer in the application.


   ## [Back](../401readingNotes.md)