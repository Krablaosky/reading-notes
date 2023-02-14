# CRUD

## [Status Codes Based on REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status code represents:

100’s = Status code 100is for when a request will fail before it sends the rest of the information 

200’s = these are our success codes This means that everything went successfully and that all requirements

300’s = this means that there is something that cannot be located,whatever they're looking for has been....to another location or does not exist

400’s = these are for invalid requests sent to a server sometimes it's missing the wrong information or authentication or missing parameters

500’s = this often is because everything is overloaded and can't beat this time

1. What is a status code 202?

a 202 success code means that the request was successfully validated and met all the requirements at the time of its sending Not that it was necessarily processed successfully

3. What is a status code 308?

this status code shows up if the resource is now available at a new URL and the client should directly access it via that new URL in the future

1. What code would you use if an update didn’t return data to a client?

the code you would use would be 204 which is no content

5. What code would you use if a resource used to exist but no longer does?

we would use the code 410 gone It's like 404 but we know that it existed in the past and that it's now no longer able to be found

6. What is the ‘Forbidden’ status code?

this means that no one has the permissions to access the resource specifically the client

## [Build a REST API with node.js](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

We want to put it in our .env file so that we can access that route and alter it from our .env file
We pull it down into our .env file so that we know which database we are accessing and what information we will need to push and pull from

2. What is middleware?

Middleware is code that runs when the server gets a request but before it gets passed to your routes

3. What does app.use(express.json()) do?

it allows our server to allow JSON as a body as opposed to a get element

4. What does the /:id mean in a route?

this is a parameter that we can access whenever someone adds that specific id to their route

5. What is the difference between PUT and PATCH?

Patch is when we want to update using only the information that the user provided us as opposed to PUT which would update all the information all at once and not just the information that was passed.

6. How do you make a default value in a schema?

you add a key value pair for default under your variables called Default and set it to your default starting information

7. What does a 500 error status code mean?

These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

8. What is the difference between a status 200 and a status 201?

The main difference between 200 and 201 is that with a 200 status everything is ok and good to go while a 201 status is used for create operations and come with a "location" header
