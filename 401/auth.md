# Authentication

## [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

1. Explain to a non-technical friend how you would safely hash and store a password.
  When it comes to safely hashing and storing passwords, the process involves using a cryptographic algorithm to convert the password into a fixed-length string of characters that cannot be easily reversed or decrypted. Here's an explanation for a non-technical friend:

  Hashing the Password: To securely hash a password, we use a strong hashing algorithm like bcrypt. Bcrypt is a widely used algorithm specifically designed for password hashing. It takes the password as input and generates a hash that is unique to that password.

  Salting the Password: In addition to hashing, we use a technique called salting. A salt is a random string of characters that is added to the password before hashing. This ensures that even if two users have the same password, their hash values will be different. Salting adds an extra layer of security to protect against attacks like rainbow tables.

  Storing the Hashed Password: Instead of storing the actual password, we only store the hashed password and the salt value. When a user tries to log in, we repeat the same process by hashing the entered password with the stored salt and compare the resulting hash with the stored hash. If they match, the password is considered valid.

2. What is Bcrypt?
  Bcrypt is commonly used for password hashing because it has several security features:

3. Why might you use something like Bcrypt?
  * Adaptive Hashing: Bcrypt is designed to be computationally expensive, which slows down the hashing process. This helps protect against brute-force attacks, where an attacker tries many possible passwords in rapid succession.

  * Salt Generation: Bcrypt automatically generates a random salt for each password, ensuring that even users with the same password will have different hashes.

  * Work Factor: Bcrypt allows you to adjust the work factor, which determines the computational cost of hashing. By increasing the work factor, you can make the hashing process even more time-consuming for attackers.


## [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

1. What is Basic Authentication?

  Basic Authentication is a straightforward method used to authenticate clients in web applications and APIs. It involves clients sending their username and password in the "Authorization" header of an HTTP request, encoded in Base64. The server decodes the credentials, verifies them against stored data, and grants access if they match. However, Basic Authentication has security limitations and should be used over HTTPS to protect the credentials from interception.

2. What properties are necessary in the header of a Basic Auth request?

  Authorization: This property contains the word "Basic" followed by the Base64-encoded string of the username and password. It is included in the "Authorization" header of the HTTP request. The format of the header is as follows:

  ```
  Authorization: Basic base64(username:password)
  ```

  The username and password are concatenated with a colon (":") separator and then encoded using Base64. This property is essential for the server to identify and authenticate the client.
  

3. How are username:password in Basic Auth encoded?

  In Basic Authentication, the username and password are encoded using Base64. The process involves concatenating the username and password with a colon (":") separator, and then applying Base64 encoding to the combined string.

  Here's an example to illustrate the encoding process:

  Suppose the username is "admin" and the password is "password123".

  Concatenate the username and password with a colon separator:

  ```
  admin:password123
  ```

  Apply Base64 encoding to the combined string:
  
  ```
  YWRtaW46cGFzc3dvcmQxMjM=
  ```
  
  The resulting encoded string, "YWRtaW46cGFzc3dvcmQxMjM=", represents the username and password in Base64 encoding. This encoded string is then included in the "Authorization" header of the Basic Authentication request.

## [OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

1. Define the authentication process to a non-technical recruiter.

  Authentication is the process of verifying a user's identity when accessing a system or application. It involves the user providing a unique identifier (like a username) and a password. The system checks if the provided credentials match the stored credentials for that user. If they match, access is granted; otherwise, it's denied. Authentication ensures that only authorized individuals can access sensitive information, helping maintain security.

2. How should your error messaging respond (both HTTP and HTML)? Why?

  Error messaging in both HTTP responses and HTML is important for providing clear feedback to users. In HTTP responses, using appropriate status codes like 401 (Unauthorized) informs the client that authentication is required. In HTML, concise and user-friendly error messages help users understand the issue and take appropriate actions to resolve it. Effective error messaging enhances user experience, aids troubleshooting, and maintains security by avoiding the disclosure of sensitive information.

3. Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.
  
  OWASP (Open Web Application Security Project) provides valuable resources and best practices for secure application development. By following OWASP fundamentals, you can reduce vulnerabilities and enhance the security of your application throughout its lifecycle. It's crucial to consider security from the inception of the development process to ensure a robust and secure authentication mechanism.