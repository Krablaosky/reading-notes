# Slate & Props

## React lifecycle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
   
Based on the diagram in the website,happens is the render phase.The render phase is pure and has no side effects It can be positive anytime or aborted or restarted. After that is the ComponentDidMount during the commit phase.

2. What is the very first thing to happen in the lifecycle of React?
   
the very first thing to happen in the life cycle of react is what's called mounting.This happens when a component is created and inserted into DOM.

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

First will be Constructor, Render, ComponentDidMount, React Updates, ComponentWillUnmount. 

4. What does componentDidMount do?

This method works immediately after a component is mounted. this usually is where you would put any information that needs to load using a network request.

## React State Vs Props

1. What types of things can you pass in the props?

types of things that you pass in props are traditionally arguments that you would normally have inside of a function. You are essentially storing all types of data that you want initially loaded. if you had a mathematical equation you would be passing integers or different variables through props.

2. What is the big difference between props and state?

the major difference between props and state is that props are things that you pass into a component. This is very different than state which is handled inside of the component and can be updated inside the component. Whereas props are handled outside of the component and have to update them outside the component.

3. When do we re-render our application?

When you change the state inside of your application it will oftentimes re-render.

4. What are some examples of things that we could store in state?

In the above example of having a mathematical equation or a function that is continually updating, as in a counter, we would use state to store those variables.Those items would be updated outside of the component every time the counter changes. if you wanted to change something in your application you would want to make sure that that data is stored in state so that way you could be updated as needed.