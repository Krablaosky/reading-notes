# AWS: API, Dynamo and Lambda

## Reading

### [AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)

1. What is Amazon API Gateway?
   * Amazon API Gateway is a fully managed service provided by AWS that enables developers to create, publish, and manage APIs for their applications. It acts as a front door for APIs, allowing easy and secure access to backend services and functions.

2. Why is Amazon API Gateway an important part of the Serverless ecosystem?
   * Amazon API Gateway is an important part of the Serverless ecosystem because it seamlessly integrates with other AWS serverless services, such as AWS Lambda, enabling developers to build and deploy serverless applications quickly. It provides features like request/response transformations, authorization and authentication, caching, and traffic management, making it a crucial component for building scalable and secure serverless architectures.

3. How does API Gateway integrate with other AWS services?
   * AWS Lambda: API Gateway can directly integrate with Lambda functions, allowing developers to trigger serverless functions in response to API requests.
   * AWS DynamoDB: API Gateway can be configured to interact with DynamoDB tables, enabling CRUD (Create, Read, Update, Delete) operations through API calls.
   * AWS Cognito: API Gateway integrates with Cognito for user authentication and authorization, allowing developers to secure their APIs and control access to resources.
   * AWS CloudWatch: API Gateway logs can be sent to CloudWatch, providing insights and monitoring capabilities for API usage and performance.
   * AWS X-Ray: API Gateway supports integration with X-Ray for distributed tracing and performance monitoring of API requests.

### [AWS API Gateway](https://aws.amazon.com/api-gateway/)

1. What are the some benefits of using Amazon API Gateway?
   * Easy API Creation and Management: API Gateway provides a simple interface to create, publish, and manage APIs, including defining endpoints, request/response mappings, and security configurations.
   * Scalability and High Availability: API Gateway automatically scales to handle varying traffic loads and provides built-in caching mechanisms to improve performance and reduce the load on backend services.
   * Security and Authorization: API Gateway supports authentication and authorization mechanisms, including API keys, IAM roles, and integration with AWS Cognito, allowing developers to secure their APIs and control access to resources.
   * API Monitoring and Analytics: API Gateway integrates with AWS CloudWatch and provides detailed logs, metrics, and tracing capabilities to monitor API usage, detect issues, and gain insights into API performance.
   * Integration with AWS Services: API Gateway seamlessly integrates with other AWS services, such as Lambda and DynamoDB, allowing developers to build powerful serverless architectures and easily connect APIs to backend resources.

2. What two API types might you choose from?
   * RESTful APIs: This type of API follows the principles of Representational State Transfer (REST), using standard HTTP methods like GET, POST, PUT, and DELETE for communication.
   * WebSocket APIs: WebSocket APIs enable real-time bidirectional communication between clients and servers, allowing applications to establish persistent connections and exchange messages in real-time.

### [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

1. What is DynamoDB?
   * DynamoDB is a fully managed NoSQL database service provided by AWS, designed for applications that require low-latency, high-scale data storage with automatic scaling and high availability.

2. Under what circumstances would you recommend DynamoDB over MongoDB?
   * DynamoDB is recommended over MongoDB in scenarios where you require a fully managed database service with seamless scalability, automatic data replication across multiple regions, and predictable performance at any scale. It excels in handling large-scale workloads with high traffic and stringent latency requirements.

### [AWS DynamoDB](https://aws.amazon.com/dynamodb/)

1. Explain to a non-technical friend how DynamoDB works.
   * DynamoDB is like a massive and fast storage system provided by AWS where you can store and retrieve data using a unique key. It automatically scales to handle any amount of data and provides consistent, low-latency performance.

### [Dynamoose](https://dynamoosejs.com/getting_started/Introduction)

1. What is Dynamoose?
   * Dynamoose is a Node.js library that simplifies working with DynamoDB by providing an easy-to-use and intuitive interface for defining and querying DynamoDB models in JavaScript.

2. What are some key features of Dynamoose?
   * Some key features of Dynamoose include automatic schema creation, model validation, support for middleware hooks, type casting,
