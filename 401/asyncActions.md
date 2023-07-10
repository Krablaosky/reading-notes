## Redux - Asynchronous Actions

### Reading

#### [async actions](https://redux.js.org/advanced/asyncactions)

1. Redux middleware is used to handle asynchronous actions in Redux. It provides a way to intercept actions before they reach the reducers, allowing for additional logic to be executed. Middleware is useful when dealing with tasks like making asynchronous API calls, handling side effects, and dispatching multiple actions based on the outcome of an asynchronous operation.

2. The Redux Async Data Flow Diagram represents the flow of asynchronous actions in Redux. Here is a description of the flow:

   1. An asynchronous action creator is called in the application code, which returns a function instead of a plain action object.
   2. The function returned by the action creator is intercepted by the Redux middleware before reaching the reducers.
   3. The middleware can perform some logic, such as making an API request or dispatching other actions, before invoking the next step.
   4. If necessary, the middleware can dispatch additional actions, such as "request started" or "request failed" actions, to update the application state accordingly.
   5. Once the asynchronous operation is complete, the inner function can dispatch a final action with the received data.
   6. The dispatched action flows through the remaining middleware (if any) and reaches the reducers, which update the application state based on the action.

3. In Redux, we can accommodate asynchronous operations by using middleware like Redux Thunk or Redux Saga. Redux Thunk is a popular middleware that allows action creators to return functions instead of plain action objects. These functions can perform asynchronous tasks, such as making API calls, and dispatch additional actions once the task is completed. Redux Thunk integrates seamlessly with Redux and provides a simple way to handle asynchronous actions in Redux applications.

#### [thunk middleware](https://github.com/reduxjs/redux-thunk)

1. Redux Thunk middleware is needed when you want to write action creators that perform asynchronous operations, such as making API requests, and need to dispatch multiple actions during the process. It allows you to add extra capabilities to your action creators by enabling them to return functions instead of plain action objects.

2. Redux Thunk middleware allows you to write action creators that return a function instead of an action. This function, known as a "thunk," can be used to delay the dispatch of an action or dispatch multiple actions based on certain conditions. The function receives the `dispatch` and `getState` functions as arguments, which can be used to dispatch actions and access the current Redux state.

3. Any return value from the inner thunk function will be made available by Redux Thunk middleware. If the inner function returns a value, it will be passed as the return value of the original dispatch call that triggered the thunk. This can be useful when working with asynchronous operations, as it allows you to handle the results or errors of the operation in the code that triggered the action.

## [Back](../401readingNotes.md)