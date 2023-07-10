# Context API

### [Choosing the State Structure](https://react.dev/learn/choosing-the-state-structure)

1. Summarize the five principles for structuring state.

The five principles for structuring state are as follows:

- Identify the minimal representation of the state: Determine the smallest possible set of data that your component needs to render and operate correctly.
- Derive additional state: If certain pieces of data can be computed based on the existing state or props, calculate and store them as derived state rather than duplicating the data.
- Identify where state should live: Decide which component should be responsible for managing and updating the state based on which component needs it the most and which components are the parents or ancestors of the components that require the state.
- Establish one-way data flow: Make sure that data flows in a single direction, from the top-down in a component tree. This makes it easier to understand and debug the state changes.
- Normalize nested state: If the state becomes complex with nested objects or arrays, consider normalizing it by flattening or restructuring the data. This simplifies state updates and reduces the chances of bugs.

### [Passing State Deeply with Context](https://react.dev/learn/passing-data-deeply-with-context)

1. What problem do Contexts aim to solve?

Contexts aim to solve the problem of prop drilling, which occurs when you need to pass data through multiple levels of nested components. Contexts provide a way to share data between components without explicitly passing it through each intermediate component in the component tree.

2. What is one technique to try before useContext?

Before using the useContext hook, one technique to try is prop drilling. Prop drilling involves passing data down through the component tree as props, even if some intermediate components don't directly use the data. While prop drilling can be a bit cumbersome, it can work well for smaller applications or when the data needs to be accessed by only a few components.

3. What hook complements useContext for complex applications?

The useReducer hook complements useContext for complex applications. While useContext provides a way to access context values, useReducer is a hook that helps manage complex state logic by providing a dispatch function and a state object. It is especially useful when the state updates involve multiple actions and complex state transitions.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

- [Sharing State Between Components](https://react.dev/learn/sharing-state-between-components)
- 
- [Preserving and Resetting State](https://react.dev/learn/preserving-and-resetting-state)

## [Back](../401readingNotes.md)