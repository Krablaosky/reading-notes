# Readings: Express REST API


## [Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

1. Classes are a template for creating objects.


2. Can a class declaration be hoisted?
  * A class declaration can not be hoisted. It is not immediately accessible in the code like function declarations.

3. How would you describe a constructor and contextual “this” to a non-technical friend?
  * A constructor is a special method within a class that is used to initialize objects created from the class. It is called automatically when a new instance of the class is created using the new keyword. The constructor allows you to set initial values or perform any necessary setup for the object. The keyword this refers to the current instance of the object being created or manipulated.

## [Using Express Routing](https://expressjs.com/en/guide/routing.html)

1. Within Express, what does routing refer to?
   * In Express, routing refers to the process of defining different endpoints (URLs) and handling HTTP requests for those endpoints. It involves mapping the requested URL to the appropriate code that will handle the request and generate a response.

2. What is the difference between a route path and a route method?
   
  * A route path in Express is the URL pattern that defines the endpoint. It can include dynamic segments and route parameters. For example, /users/:id defines a route path with a dynamic segment :id that can match any value.

3. When is it appropriate to add `next` as a parameter to a route handler and what must you do if `next` has been passed to your middleware as a parameter?
   * A route method in Express refers to the HTTP method (e.g., GET, POST, PUT, DELETE) associated with a route. It determines what kind of operation will be performed on the specified endpoint.

    * It is appropriate to add next as a parameter to a route handler when you want to pass control to the next middleware function in the chain. If next is passed to your middleware as a parameter, you must invoke it within your middleware function to pass control to the next function.

## [Express Routing](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4)

1. What is an Express Router?
   * An Express Router is a mini express application that can be used to handle routes separately from the main express application. It allows you to modularize your routes and create a more organized code structure.

2. By what mean do we initialize `express.Router()` in an express server?
   * express.Router() is initialized in an express server by creating a new instance of the router using the express.Router() function and assigning it to a variable. For example:
  ``` javascript
  const express = require('express'); 
  const router = express.Router();
  ```
3. What do we use route middleware for?
   * Route middleware is used to perform operations on a specific route or a group of routes. It can be used to add additional functionality or perform tasks such as validation, authentication, logging, etc. before or after handling the actual request.


## Reflection

What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-03/)?

My learning goals are to understand how to break roots up into much more efficient and logical ways.I'm really hoping to reinforce my understanding of CRUD and REST operations, As well as get better at building efficient routes.I still feel like I could use more practice with building more routes And how to use the SQL database with Postgres. I still haven't been able to get that configured. I'm excited to understand how to use SQL databases better with our javascript applications and I am excited to see where we can go with this.