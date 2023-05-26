# Event Driven Applications

### [Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

1. What native Node.js module allows us to get started with Event Driven Programming?
   * The native Node.js module that allows us to get started with Event Driven Programming is called `events`. It provides an EventEmitter class that enables us to create and handle custom events in our Node.js code.

2. What is the value of Object Oriented Programming used in tandem with Event Driven Programming?
   * The value of Object-Oriented Programming (OOP) used in tandem with Event Driven Programming lies in code organization, maintainability, and reusability. OOP helps structure code into modular and reusable components called objects. These objects encapsulate data and behavior, promoting code organization and making it easier to maintain and extend.
   * In the context of Event Driven Programming, OOP allows us to define objects that can emit events and handle them accordingly. By encapsulating event-emitting and event-handling logic within objects, we can achieve a more structured and modular approach. This makes it easier to understand, maintain, and modify code, as each object can have its own set of events and associated behaviors.

3. Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.
   * Imagine you have a website where users can sign up, log in, and perform various actions. On the frontend, Event Driven Programming is commonly used to handle user interactions like button clicks, form submissions, or mouse movements. Similarly, on the backend using Node.js, Event Driven Programming can be valuable.
   * Node.js is well-suited for building scalable and efficient backend systems, and Event Driven Programming is a fundamental practice in Node.js development. With Event Driven Programming on the backend, your Node.js server can listen for events like incoming requests, database operations completing, or external services sending data.

   * By leveraging Event Driven Programming on the backend, you can design your server to be highly responsive and handle multiple requests simultaneously. When an event occurs, (i.e. a request arriving) the server can trigger the appropriate event handler to process the request, fetch data from databases, perform computations, or communicate with other services.

   * This asynchronous approach allows the server to efficiently handle multiple requests without blocking the execution of other code. It enables your Node.js server to handle real-time applications, chat systems, websockets, or any scenario where responsiveness and scalability are crucial.

   * Overall, Event Driven Programming in the backend using Node.js helps you build highly scalable and responsive systems by allowing your server to react to events in an efficient and non-blocking manner, providing a solid foundation for building powerful web applications and services.