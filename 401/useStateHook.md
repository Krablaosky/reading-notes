# useState() Hook

## Reading

### [Thinking in React](https://react.dev/learn/thinking-in-react)

1. Summarize the five steps of thinking in react.
  Certainly! Here are the five steps of thinking in React in Markdown format:
   * **Break the UI into a component hierarchy**: Start by breaking down the user interface into smaller, reusable components. Identify the different parts of the UI and determine which components can be created to encapsulate their functionality.
   * **Build a static version of the UI**: Construct a static version of the UI using the components created in the previous step. This version should take props but have no interactivity yet. Focus on building the structure and appearance of the UI.
   * **Identify the minimal, but complete, representation of UI state**: Determine the minimal set of mutable state that the UI requires. Think about which components need to have state and what data should be stored in that state. Remember that state should be minimal and contain only the necessary data for rendering the UI.
   * **Identify where your state should live**: Find the common parent component that should own and control the shared state. This component should be the highest component in the hierarchy that needs access to the state. It will pass the state down to child components through props.
   * **Add inverse data flow**: Implement the interactivity by adding event handlers to the components. These event handlers should modify the state and trigger re-rendering of the components. Ensure that the data flow is inverse, meaning the state is owned by the common parent component and passed down to child components. This allows the child components to update the state indirectly through callbacks, maintaining a unidirectional flow of data.

### [State: A Component’s Memory](https://react.dev/learn/state-a-components-memory)

1. What is one reason a local variable isn’t sufficient for managing a React component?
   * One reason a local variable isn't sufficient for managing a React component is that local variables are not persistent across component renders. When a component re-renders, the local variables are re-initialized, losing their previous values. This can lead to the loss of important data or the inability to maintain the component's state between renders. In React, state management solutions like React's `useState` hook or state stored in a parent component provide persistence and ensure that the component retains its state even after re-renders.

2. What is the argument to the useState hook, and what are the two parts of its return array?
   * The argument to the `useState` hook is the initial value of the state. It is passed as an argument when calling the `useState` function. The `useState` hook returns an array with two elements:

   - The first element is the current state value, which can be accessed and updated.
   - The second element is a function that allows you to update the state. By invoking this function and passing a new value, React will re-render the component with the updated state.

   The syntax for using `useState` is as follows:

   ```jsx
   const [state, setState] = useState(initialValue);
   ```

3. How can Component A access state from Component B?
   * To access state from Component B in Component A, you need to lift the state up to a common ancestor component that is higher in the component hierarchy and has both Component A and Component B as descendants. This common ancestor component should hold the shared state in its own local state using a state management solution like React's `useState` hook. Then, the shared state can be passed down to Component A and Component B as props. Component A can access the shared state by receiving it as a prop and using it within its own component logic. This way, both components can access and utilize the shared state, enabling communication and data sharing between them.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

[Passing Props to a Component](https://react.dev/learn/passing-props-to-a-component)

[Rendering Lists](https://react.dev/learn/rendering-lists)

[State as Snapshot](https://react.dev/learn/state-as-a-snapshot)

[useState hook](https://react.dev/reference/react/useState)