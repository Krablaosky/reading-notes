# AWS: Events

## Reading

### [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

1. What is the difference betweeen SQS and SNS?
   * The main difference between Amazon Simple Queue Service (SQS) and Amazon Simple Notification Service (SNS) is their messaging pattern and delivery mechanism. SQS is a fully managed message queuing service that decouples the components of a distributed system by allowing asynchronous communication, while SNS is a publish-subscribe messaging service that delivers messages to multiple subscribers simultaneously.

2. What are some use cases for both SNS and SQS?
   * Use cases for SQS:
     * Workload Decoupling: SQS enables decoupling of components in a distributed system, allowing different parts of an application to communicate asynchronously and independently, reducing dependencies and improving scalability.
     * Task Processing: SQS can be used to distribute and process tasks or messages across multiple workers or systems, ensuring reliable and efficient task handling.
     * Event Sourcing: SQS can be used to handle event-driven architectures, where events are stored in a queue and processed asynchronously by subscribers.
     * Delayed Processing: SQS provides support for delayed delivery of messages, allowing delayed processing or scheduling of tasks.

   * Use cases for SNS:
      * Pub/Sub Messaging: SNS facilitates pub/sub messaging patterns, where a single message can be published to multiple subscribers simultaneously.
      * Notifications and Alerts: SNS is commonly used for sending notifications and alerts to multiple endpoints or subscribers, such as email, SMS, mobile push notifications, or HTTP endpoints.
     * Event-driven Architectures: SNS is suitable for event-driven architectures, where events need to be broadcasted to multiple subscribers for real-time processing or analysis.
     * Fanout Pattern: SNS can be used in the fanout pattern, where a single message is published to an SNS topic and delivered to multiple SQS queues or other endpoints. 

### [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

1. Describe how to use SQS and SNS in a “fanout” pattern.
   * In a "fanout" pattern, you can use SNS and SQS together by subscribing multiple SQS queues to an SNS topic. When a message is published to the SNS topic, it gets delivered to all the subscribed SQS queues, allowing each queue to independently process the message.

2. Explain how “push notifications” work, using SNS.
   * Push notifications work using SNS by allowing publishers to send messages to subscribers asynchronously. Publishers send messages to SNS topics, and subscribers (such as mobile devices or application endpoints) subscribe to these topics. When a message is published to a topic, SNS delivers it to all the subscribed endpoints, which can receive the message as a push notification.

### [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

1. How might a large scale, distributed application make use of a Queue system like SQS?
   * In a large-scale, distributed application, SQS can be used as a queue system to handle incoming requests or tasks. Different components or services of the application can send messages to an SQS queue, and worker processes can pull messages from the queue for processing. This allows for parallel and asynchronous processing, as the workers can scale independently based on the message load and handle tasks in a distributed manner, improving performance and scalability. It also provides fault tolerance and ensures that no messages are lost even if a worker or component goes down.


## Bookmark and Review

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)