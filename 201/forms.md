# Building forms in HTML, CSS, and JS

## HTML Forms

Forms are pretty critical to building a website. Most websites use forms in one way or another and there can be so many uses for them while we dig into building robust and complex websites.

1. Why are forms so important in web development?

Forms are important for websites for building things like logins, shopping orders, or in general collecting data from users. It's an integral way of building user interfaces and play a huge role in most websites. 

2. When designing a form, what are some key things to keep in mind when it comes to user experience?

It's pretty key to wire frame out what you want the form to look like so that it makes coding easier. You don't want the form to be too big and complicated as that might frustrate users. Keep the data collected to be as concise as possible.

3. List 5 form elements and explain their importance.

Form elements are more complex than most html elements.
One of our elements is the `input` element which takes in information like text entries, numbers, or dates. There is also a `button` element which is usually a clickable element that the user can interact with to activate the information or run a function.
We also frequently use the `form` element to create forms that users can enter data into like their login information. The `fieldset` element is frequently used to group several controls and labels within a webform. It also often gives structure to the webform.
Finally we have the `label` element  which often times is used in forms to place the title of the fillable form on top of or to the side of the box. These elements are used every day and we don't often realize how prevalent they are.

## JS Introduction To Events.

1. How would you describe events to a non-technical friend?

Think of an event as a situation that happens. When The traffic light turns green you know to go, and when it turns red you know to slow down. These color `events` inform what we are going to do and let us know what should happen.

2. When using the addEventListener() method, what 2 arguments will you need to provide?

When using event listeners, which in the case of our above example would be your eyes. They take in the light color and then know what to do with it from there. For that we need to register the event thats happening and the code for whats going to happen. We don't want to start running or going everytime we see the color green. Only when we are in the car and that specific event is occuring.

3. Describe the event object. Why is the target within the event object useful?

An event object is the event that gets passed in from the event listener and helps run the code function we want. We pass that parameter into the function and can manipulate that data from there. When we use the `.target` code on our event, it helps to narrow down what type of data we are trying to manipulate.

4. What is the difference between event bubbling and event capturing?

These two terms talk about how browsers will handle events when they are nested elements. Event bubbling takes the inner nested target and applies it to the elements parents and runs it for them as well. Think of it like starting at the bottom and bubbling up to all of the containers. On the other end of this the event capture checks to see if the outer most element has a `click` event and then keeps moving inwards until it reaches the direct parent of the element that was actually clicked.