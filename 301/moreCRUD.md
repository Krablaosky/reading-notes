#  More CRUD

## [CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

1. Which HTTP method would you use to update a record through an API?

If we Wanted to update a record through an API We would use a PUT method

2. Which REST methods require an ID parameter?

the two rest methods that require ID parameters are the update method where we want to be able to specifically target which item we are updating. The same thing goes for the delete method for the exact same reason

## [Speed Coding, Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

1. What’s the relationship between REST and CRUD?

REST is an architectural system centered around resources where we use HTTP commands to be able to access them and CRUD is a cycle meant to maintain records and database setting. So for us CRUD is a way of manipulating information and REST is controlling the data through HTTP commands. CRUD can operate with an arrest architecture but REST API's can exist independently of CRUD

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

- Identify the resources: The first step in creating a RESTful API is to identify the resources that the API will expose. Resources can be anything from data entities such as users, orders, or products to more abstract concepts such as messages or notifications.

-Define the endpoints: Once you have identified the resources, the next step is to define the endpoints that the API will expose for each resource. Such as /users or /orders/123.

-Choose the HTTP methods: RESTful APIs use HTTP methods to indicate the type of operation being performed on a resource. The most common HTTP methods used in RESTful APIs are GET, POST, PUT, PATCH, and DELETE. Choose the appropriate HTTP method for each endpoint based on the operation being performed.

-Design the response format: RESTful APIs typically return data in a standardized format such as JSON or XML. You will need to design the response format for each endpoint and ensure that the data returned is consistent with the expectations of your clients.

-Implement the API: Once you have designed the API, the final step is to implement it. This involves writing the code that handles incoming requests, processes data, and returns responses in the expected format. You may also need to implement authentication and authorization mechanisms to ensure that only authorized clients can access the API.

