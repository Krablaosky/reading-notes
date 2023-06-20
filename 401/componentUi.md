# Component Based UI

## Reading 

### [React Quick Start](https://react.dev/learn)

Read the React Quick Start quide, to refresh your memory on React.

1. What are the building blocks of a React app?
   * The building blocks of a React app are components. Components are reusable, self-contained pieces of code that can be composed together to build complex user interfaces.

2. What is the difference between an HTML element and a React component?
   * An HTML element represents a specific element in the HTML document structure, such as `<div>`, `<p>`, or `<span>`. On the other hand, a React component is a JavaScript function or class that returns JSX (JavaScript XML) to describe the structure and appearance of a part of the user interface. While HTML elements are static and defined by the HTML specification, React components are dynamic and can have their own logic and state. 

3. What is JSX and why do we use it?
   * JSX is a syntax extension for JavaScript that allows you to write HTML-like code in JavaScript. It provides a way to describe the structure and appearance of UI components in a declarative manner. JSX is not required to use React, but it is a popular and convenient choice because it enables you to write component templates in a familiar HTML-like syntax.


4. Describe the process of embedding JavaScript expressions in JSX.
   * JavaScript expressions can be embedded in JSX by wrapping them in curly braces `{}`. For example, if you want to display the value of a variable `name` in JSX, you can write `{name}`. This allows you to dynamically compute and display values based on the state or props of the component.

5. Does React or JSX have any special features for iteration or conditional logic?
   * Yes, both React and JSX provide special features for iteration and conditional logic. In React, you can use JavaScript's map function or the JSX spread syntax `(...)` to iterate over an array of data and dynamically render components. For conditional rendering, you can use JavaScript's conditional statements (if, ternary operator) within JSX to conditionally render different parts of the UI based on certain conditions.

6. How does React know to respond to a user’s inputs?
   * React responds to a user's inputs through event handling. You can attach event handlers to React components using special props, such as `onClick`, `onChange`, etc. When an event occurs, React invokes the corresponding event handler function, which can then update the component's state or trigger other actions.

7. What word indicates that a React component manages data with a Hook?
   * The word that indicates that a React component manages data with a Hook is "useState". Hooks are functions that allow you to use state and other React features in functional components. `useState` is a Hook that enables you to add state to a functional component.


8. How can two react components share data?
   * Two React components can share data by lifting the shared state up to their common ancestor component. This means that the state is stored in a higher-level component, and the child components receive the shared data through props. When the shared state is updated, the changes propagate down the component tree, triggering re-rendering of the affected components with the updated data. This technique is known as "lifting state up" or "state lifting."

### [Render and Commit](https://react.dev/learn/render-and-commit)

1. What are the three steps of refreshing a React UI?
   *  **Render**: In this step, React builds a virtual representation of the UI based on the component hierarchy and their current state and props. This virtual representation is called the virtual DOM.
   *  **Commit**: Once the virtual DOM is created, React compares it with the actual DOM and determines the minimal set of changes required to synchronize them.
   *  **Apply Changes**: In this final step, React applies the necessary changes to the actual DOM, updating only the elements that have changed. This ensures efficient and optimized updates to the UI.


2. How do you trigger updates to a component after the initial render?
   * Updates to a component can be triggered by changes in its state or props. After the initial render, React automatically handles the updates when there are changes in the component's state or when new props are passed to it. React compares the previous state/props with the new state/props and re-renders the component if there are differences. This triggers the component's `render` method to be called again, generating a new virtual DOM representation and eventually updating the actual DOM.

3. Does React recreate DOM nodes on every rerender?
   * No, React does not recreate DOM nodes on every rerender. Instead, it performs a diffing algorithm to determine the minimal set of changes needed to update the DOM. It compares the previous virtual DOM representation with the new one and identifies the differences. Based on these differences, React applies only the necessary changes to the actual DOM, such as adding, removing, or updating specific elements. This approach is more efficient than recreating the entire DOM on every rerender.

4. After React has updated the DOM, what still needs to happen before the user sees the change?
   * After React has updated the DOM, the changes are not immediately visible to the user. The browser needs to perform the painting and layout process before the user sees the updated UI. This process involves converting the updated DOM into pixels on the screen. Additionally, if there are any CSS transitions or animations involved, they may need to be executed before the user perceives the changes. Once the painting, layout, and any transitions are complete, the user can finally see the updated UI on their screen.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

[Your First Component](https://react.dev/learn/your-first-component)

[Importing and Exporting Components](https://react.dev/learn/importing-and-exporting-components)

[Writing Markup with JSX](https://react.dev/learn/writing-markup-with-jsx)

Cheat sheets

[sass cheatsheet](https://devhints.io/sass)
[react cheatsheet](https://devhints.io/react)