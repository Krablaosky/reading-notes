# Thinking in React and putting it all together

## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components?

Single responsibility principle in terms of components, is about simplifying each component. Each component should only be responsible for one thing, if it does get larger it be broken up into smaller sub-components instead of one large section of code that continues to get bigger and bigger.

2. What does it mean to build a ‘static’ version of your application?

When we build a static version of our application, we're referencing an application that only involves text and is not interactive. essentially want to use props to display the information that we have, we don't want to have a fluctuating state that is going to update all of that information.

3.  Once you have a static application, what do you need to add?

Once we have a fully complete static application we need to start thinking about interactivity,and how we're gonna use `state` to accomplish that.

4. What are the three questions you can ask to determine if something is state?

The three questions we need to ask ourselves to figure out if something need to be state are the following

```
1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.
```

5. How can you identify where state needs to live?

one of the most important pieces about state is that it is one way data flow,does must follow and adhere to our component hierarchy.In order to figure out where states should belong we need to identify each component that renders something and the common component above all of them that needs that state to be able to feed it back down as a prop

## [Higher Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?

a higher order function is a function that takes in other functions as arguments or returns them,Higher order functions allow us to iterate over functioning actions not just values.

2.  Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

the second line in the greater than function,is returning another function that determines if M is greater than N, if it is then it will return M.

3. Explain how either map or reduce operates, with regards to higher-order functions.

are map and reduce functions operate by transforming an array by applying a function to each element And then it builds a brand new array from the return to values. the content is going to look different than the original input. in the instance of our reduce function,we would take the initial array and then we would add the next object value to a brand new array and then continues down the line creating that new value for the new array based on the old elements of the old array.