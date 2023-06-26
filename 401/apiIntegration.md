## Reading

### Review API Server Build

1. **Explain the difference between a query string parameter and a path parameter.**

   A query string parameter is used to pass additional information to a server as part of the URL. It appears after the `?` symbol in the URL and consists of key-value pairs separated by `&` symbols. Query string parameters are optional and can be used to filter or modify the data returned by the server. For example, in the URL `http://our-site.com/api/products?category=electronics`, the `category=electronics` is a query string parameter.

   On the other hand, a path parameter is a part of the URL path itself and is used to identify a specific resource or endpoint. Path parameters are essential for defining the structure and hierarchy of the API. They are denoted by a placeholder value within curly braces `{}` in the URL. For example, in the URL `http://our-site.com/api/products/{id}`, the `{id}` is a path parameter that represents a unique identifier for a specific product.

2. **What would our API URL with a path id parameter be given the following information:**
   - Domain: http://our-site.com
   - v3
   - Model name: stuff
   - id: things

   The API URL with a path id parameter would be: `http://our-site.com/v3/stuff/things`

3. **We have created a dynamic API with an "interface". Describe how that interface works to a non-technical friend.**

   Imagine you have a digital assistant that helps you interact with different services. This assistant has a menu or a set of buttons that represent various functions or tasks you can perform. Each button is like an interface that you can click on to make something happen.

   In the context of a dynamic API, the "interface" refers to a set of predefined endpoints or routes that the API exposes. These endpoints are like buttons that you can call or interact with to perform specific actions or retrieve specific information. For example, if you have an e-commerce API, the interface could include endpoints like `/products` to retrieve a list of products, `/orders` to place an order, or `/users` to manage user-related operations.

   When you send a request to a specific endpoint, the API understands which button you pressed and performs the corresponding action. It retrieves the requested data, saves it to a database, or carries out any other necessary task. The interface acts as a bridge between your application and the API, allowing you to access and manipulate the data and services provided by the API in a structured and controlled manner.


### Review Auth Server Build

1. **Describe how you would use middleware to implement basic and bearer auth.**

   Middleware plays a crucial role in implementing authentication mechanisms in a server application. Here's how middleware can be used to implement basic and bearer authentication:

   - Basic Authentication: 
     1. The server receives an incoming request.
     2. The middleware intercepts the request before it reaches the intended endpoint or route.
     3. The middleware checks if the request contains the necessary credentials, typically in the form of a username and password. These credentials are often provided as a base64-encoded string in the `Authorization` header of the request.
     4. If the credentials are valid, the middleware allows the request to proceed to the intended endpoint or route. Otherwise, it returns an error response, indicating that the request is unauthorized.

   - Bearer Authentication:
     1. The server receives an incoming request.
     2. The middleware intercepts the request before it reaches the intended endpoint or route.
     3. The middleware checks if the request contains a valid access token, typically provided in the

 `Authorization` header as a bearer token.
     4. The middleware verifies the validity of the access token, usually by checking its signature or consulting an authentication server.
     5. If the token is valid, the middleware allows the request to proceed to the intended endpoint or route. Otherwise, it returns an error response, indicating that the request is unauthorized.

   Middleware acts as a gatekeeper, ensuring that only authenticated and authorized requests are allowed to access protected resources within the server application.

2. **Describe the handshake necessary to implement OAuth.**

   OAuth is an authentication protocol used by applications to grant limited access to user accounts on other services, without exposing the user's credentials. Here's a simplified description of the handshake process involved in implementing OAuth:

   1. The user initiates the OAuth process by clicking on a "Sign in with [Provider]" button on a third-party application.
   2. The user is redirected to the authentication server of the provider (e.g., Google, Facebook, or Twitter).
   3. The user is prompted to enter their login credentials on the provider's authentication page.
   4. Once the user is authenticated by the provider, the provider generates an authorization code.
   5. The user is redirected back to the third-party application with the authorization code as a query parameter.
   6. The third-party application sends a request to the provider's token endpoint, along with the authorization code, client ID, client secret, and a redirect URI.
   7. The provider verifies the information and returns an access token and, optionally, a refresh token to the third-party application.
   8. The third-party application can then use the access token to make authorized API requests on behalf of the user.
   9. The access token may have an expiration time. If it expires, the third-party application can use the refresh token to obtain a new access token without requiring the user's involvement.

   This handshake process allows the third-party application to obtain an access token from the authentication server, which can be used to access limited resources on behalf of the user, without directly exposing the user's credentials to the third-party application.

3. **Describe how Role-Based Access Control works to a non-technical friend.**

   Role-Based Access Control (RBAC) is like having different keys that grant access to different parts of a building. In a building, you have different rooms, and some rooms are restricted and can only be accessed by specific people. RBAC works in a similar way but in the context of computer systems and applications.

   Imagine you have an application with many users, and each user has a specific role assigned to them. These roles define what actions a user can perform and what information they can access within the application.

   For example, consider a school management system:
   - The principal has an "Administrator" role and can perform all actions within the system, such as creating accounts, managing teachers, and viewing students' records.
   - Teachers have a "Teacher" role and can perform actions like grading assignments, marking attendance, and viewing student progress.
   - Students have a "Student" role and can view their own grades, assignments, and attendance but cannot modify any information.

   In RBAC, the system administrator assigns each user a specific role based on their responsibilities and permissions. This determines what they can and cannot do within the application. The roles act as access levels that control the user's actions and limit their access to certain features or data.

   RBAC provides a structured and organized approach to managing access and maintaining security within an application. It ensures that users can only perform actions and access information that is appropriate for their role or position, thereby safeguarding sensitive data and preventing unauthorized actions.