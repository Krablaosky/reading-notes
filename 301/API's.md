# API's


1. What does REST stand for?

REST Stands for representational state transfer, it's essentially an architectural approach to designing web services

2. REST APIs are designed around a ____.

rest APIS are designed around resources which are objects data or services that can easily be accessed by clients

3. What is an identifier of a resource? Give an example.

identifiers are urls that uniquely identify different resources,different urls might take you to different parts of a webpage or different resources From a site

1. What are the most common HTTP verbs?

the most common HTTPverbs getget, post, put, patch and delete

5. What should the URIs be based on?

URIS should be based on nouns or resources And not verbs which are the operations on the resources

6. Give an example of a good URI.

This is an example of a good versus a bad URI
```
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid
```

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

having a chatty API is when there are more requests that impose a huge load on a web server,This can send multiple requests to find all of the data requires and can overload the server.

8. What status code does a successful GET request return?

a successful get request will return the status code of 200 or OK

9. What status code does an unsuccessful GET request return?

when get requests are unsuccessful you will oftentimes get the most common error message which is 404 not found

10.  What status code does a successful POST request return?

If you have a successful post method it will create a new resource which returns the status code 201 or created

11.  What status code does a successful DELETE request return?

A successful delete operation will respond with the status code of 204 meaning no content. it indicates that that process has been successfully completed and the response contains no further information.

