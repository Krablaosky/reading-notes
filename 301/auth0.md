# Authentication

## [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth?

OAuth is standard authorization protocol or framework that Describes how unrelated servers and services can access authenticated assets without actually sharing login credentials Essentially it's login protection

2. Give an example of what using OAuth would look like.

using Oauth would be similar to clicking on the sign in with Google Facebook or another service to a website.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

It works by essentially taking the already approved and accessed credentials and using them to access another service saying that this is definitively this user and everything should be OKAY. basically the first site connects to the second on behalf of the user Then the second side generates a one time use token with a secret transaction ID. the first site gives this token and the client software presents the request token. at this point the client the client may be asked to authorize and authenticate this transaction and approve it. Once approved then the user has access to the second site on behalf of the first sites authentication 

4. What is OpenID?

open ID is for humans logging into machines while Oauth is for machines logging the machines on behalf of people.

[Authorization and Authentication Flows](https://auth0.com/docs/flows)

1. What is the difference between authorization and authentication?

Authentication is the process of verifying the identity of a user or system. This is typically done by requiring the user to provide some form of credentials, such as a username and password, which are then compared to a known set of valid credentials. If the credentials match, the user is considered authenticated and granted access to the system or resource.

Authorization, on the other hand, is the process of determining whether an authenticated user has the necessary permissions to perform a specific action or access a specific resource. This can be done by checking the user's credentials against a set of predefined access control rules, which specify which users are allowed to do what.

2. What is Authorization Code Flow?

Authorization Code Flow is an OAuth authorization flow that is used to obtain an access token on behalf of a user. It is the most secure and commonly used OAuth flow for server-side web applications and native mobile applications.

The flow works as follows:

The user initiates an authentication request to the authorization server by clicking on a login button on the client application.

The authorization server redirects the user to a login page where the user enters their credentials.

The authorization server authenticates the user and generates an authorization code, which is a short-lived code that is used to obtain an access token.

The authorization code is returned to the client application via a callback URL.

The client application then makes a back-end call to the authorization server, passing the authorization code along with the client credentials (client ID and client secret) to request an access token.

The authorization server verifies the authorization code and client credentials, and if they are valid, issues an access token to the client application.
The client application can then use the access token to access protected resources on behalf of the user.

The Authorization Code Flow is more secure than other OAuth flows because the access token is never exposed to the user or the client application. Instead, the client application only receives an authorization code that can be exchanged for an access token. This helps to prevent unauthorized access to the user's data and reduces the risk of token theft.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

The Authorization Code Flow with PKCE works as follows:

The client application generates a random value called a "code verifier" and hashes it using a cryptographic hash function to create a "code challenge."

The client application initiates an authentication request to the authorization server, including the code challenge in the request.

The authorization server returns an authorization code to the client application after the user successfully authenticates.

The client application then makes a back-end call to the authorization server, passing the authorization code along with the code verifier.

The authorization server verifies the authorization code and code verifier by hashing the code verifier using the same cryptographic hash function and comparing it to the code challenge that was included in the initial request. If they match, the authorization server issues an access token to the client application.

4. What is Implicit Flow with Form Post?

 the Implicit Flow with Form Post works as follows:

The client application initiates an authentication request to the authorization server, including the requested scopes and a redirect URL in the request.

The authorization server authenticates the user and issues an access token and a refresh token, and returns them to the client application in a form post response. The response is an HTML form that is automatically submitted by the browser using a POST method, with the access token and refresh token included in the form fields.

The client application extracts the access token and refresh token from the form fields and stores them in the browser's local storage or session storage.

The client application can then use the access token to access protected resources on behalf of the user.

5. What is Client Credentials Flow?

The Client Credentials Flow works as follows:

The client application sends a request to the authorization server, including its client ID and client secret in the request headers.

The authorization server authenticates the client application using the client credentials and issues an access token to the client application.

The client application can then use the access token to access protected resources on behalf of itself.

6. What is Device Authorization Flow?

The Device Authorization Flow works as follows:

The device sends an authorization request to the authorization server, including its client ID and a requested scope in the request.

The authorization server responds with a device code and a verification URL, which the user must use to authorize the device.

The user navigates to the verification URL on another device, such as a smartphone or laptop, and enters the device code that was provided by the device.

The authorization server verifies the device code and user authorization and issues an access token to the device.

The device can then use the access token to access protected resources on behalf of the user.

7. What is Resource Owner Password Flow?

The Resource Owner Password Flow works as follows:

The client application requests the user's username and password, and sends them to the authorization server along with its client ID and client secret.

The authorization server authenticates the user's credentials and issues an access token to the client application.

The client application can then use the access token to access protected resources on behalf of the user.
