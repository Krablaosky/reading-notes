# Login and Auth

### [What is Role Based Access Control (RBAC)?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

1. What is Role Based Access Control (RBAC)?

   Role Based Access Control (RBAC) is a security model that provides a structured approach to managing user access rights in a system. It assigns roles to users based on their responsibilities and then grants permissions to those roles. RBAC simplifies access control by organizing user permissions around roles rather than individually assigning permissions to each user. It helps ensure that users only have the necessary privileges to perform their specific tasks, promoting security, and reducing administrative overhead.

2. Share an example of RBAC including all possible CRUD operations and correlating roles.

   Example: Consider a blogging platform with three roles: Admin, Editor, and Author. Each role has different levels of access and permissions.
   
   - Admin role:
     - Create, Read, Update, and Delete (CRUD) operations on all blog posts and user accounts.
   
   - Editor role:
     - Create, Read, Update, and Delete (CRUD) operations on all blog posts.
     - Read-only access to user accounts.
   
   - Author role:
     - Create and Read operations on their own blog posts.
     - Read-only access to all other blog posts and user accounts.

3. What are the benefits of RBAC?

   Some benefits of RBAC include:
   - Simplified access control: RBAC provides a structured and centralized approach to managing user access, making it easier to assign and revoke permissions based on roles.
   - Reduced administration overhead: With RBAC, managing user permissions becomes more efficient as roles can be assigned to multiple users simultaneously.
   - Enhanced security: RBAC ensures that users only have access to the resources necessary for their roles, reducing the risk of unauthorized access or privilege misuse.
   - Scalability: RBAC accommodates organizational growth by allowing the creation of new roles and easily assigning permissions to those roles, without impacting existing user permissions.
   - Compliance and auditability: RBAC helps meet regulatory and compliance requirements by providing a framework for assigning and documenting user access rights.

### Compare and Contrast the following two Libraries:

[react-cookie library](https://www.npmjs.com/package/react-cookie)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

1. Describe some react-cookie features.

   The react-cookie library provides a simple API to manage cookies in a React application. Some features of react-cookie include:
   - Setting and getting cookies: It provides methods like `set`, `get`, and `remove` to manage cookies easily.
   - Cookie persistence: The library handles cookie expiration and persistence automatically, allowing you to set the cookie's expiration time or make it a session cookie.
   - Server-side rendering (SSR) support: react-cookie supports server-side rendering, ensuring that cookies work correctly in both client and server environments.
   - TypeScript support: The library has TypeScript declarations, providing type safety when using it in TypeScript projects.
   
2. Describe some react-cookies features.

   The react-cookies component is a lightweight cookie management solution for React applications. Some features of react-cookies include:
   - Reading and writing cookies: It provides functions like `load`, `save`, and `remove` to read, write, and delete cookies.
   - Cookie options: react-cookies allows you to set options for cookies, including path, domain, expiration time, and secure flag.
   - TypeScript support: The library includes TypeScript definitions, enabling type checking and autocompletion for TypeScript projects.
   - Compatibility: react-cookies is compatible with both client-side and server-side rendering (SSR)

 environments.
   
3. Which library would you prefer? Why?
  
  I prefer to use the react-cookies library because at this time I really appreciate straightforward API usage and integration. Once I feel more comfortable with API integrations and componetization I would probably lean towards the react-cookies components to be able to modularize and keep it efficient.