# AWS: Cloud Servers

## Reading

### [AWS EC2](https://aws.amazon.com/ec2/)

1. What is an EC2 Instance?
   * An EC2 instance is a virtual server in Amazon Web Services (AWS)'s Elastic Compute Cloud (EC2) service. It provides scalable computing capacity in the cloud and allows users to launch and manage virtual machines (instances) with different configurations, such as varying processing power, memory, storage, and networking capabilities.

2. Name 2 use cases for EC2.
   * Two common use cases for EC2 instances are:
      - a. Web Hosting: EC2 instances can be used to host websites and web applications. Users can configure and manage the virtual server according to their requirements, including installing necessary software, setting up databases, and scaling resources to handle varying levels of web traffic.

      - b. Big Data Processing: EC2 instances are often employed for big data processing tasks such as data analytics, data warehousing, and large-scale data processing. EC2 provides the flexibility to deploy and manage instances optimized for handling these compute-intensive workloads.

3. Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.
   * One reason to use Amazon Elastic Container Service (ECS) instead of a service like Heroku, Digital Ocean, or Render.com is the seamless integration with other AWS services. ECS is designed to work well within the AWS ecosystem, allowing easy integration with services such as Amazon S3 for storage, Amazon RDS for databases, and Amazon CloudWatch for monitoring and logging. If your application relies heavily on other AWS services or you require a high level of customization and control over your infrastructure, ECS can provide a more integrated and comprehensive solution compared to third-party platforms like Heroku, Digital Ocean, or Render.com.

### [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

1. Where can we find EC2 on the AWS Console?
    a. Open the AWS Management Console in your web browser.

    b. Sign in to your AWS account.
  
    c. In the AWS Management Console dashboard, you can either search for "EC2" in the search bar at the top, or you can navigate to the "Compute" section and select "EC2" from the services list.

2. Explain the general difference between T2 Micro and XL.
   * T2 Micro and XL are both instance types within the EC2 service, but they differ in terms of their specifications and capabilities:
  
    * T2 Micro: T2 instances are "burstable performance instances" designed for workloads that don't require continuous high CPU performance. T2 Micro is the smallest and most cost-effective T2 instance size. It offers a single virtual CPU (vCPU) and a limited amount of memory, making it suitable for low-traffic applications or development environments with minimal resource requirements.

   * XL (Extra Large): XL typically refers to an instance type with larger specifications compared to T2 Micro. The "XL" in this context may be associated with different instance families, such as the general-purpose M5 or the memory-optimized R5. These instance types provide higher computational power, more vCPUs, and greater memory capacity, making them suitable for demanding workloads or resource-intensive applications.

   * In summary, T2 Micro is a smaller, cost-effective instance type suitable for low-resource applications, while XL refers to a larger and more powerful instance type with greater capabilities for resource-intensive workloads.

3. Explain a “Compute Cycle” to a non-technical friend.
   * To explain a "Compute Cycle" to a non-technical friend, you can use an analogy:

   * Think of a compute cycle as a single task or operation that a computer processor performs. It's like a cooking recipe. When you cook a meal, you have different steps to follow, such as chopping vegetables, boiling water, and simmering the sauce. Each step takes some time to complete, and when you finish one step, you move on to the next.

   * Similarly, a compute cycle is like a step in a recipe, but instead of cooking, it's the process that a computer's processor goes through to perform tasks. The processor executes instructions and calculations, like adding numbers or processing data. Each compute cycle represents one of these steps, and the processor completes many cycles in a second to perform complex computations or run software.

   * Just as a recipe can have multiple steps, a computer program or task may require many compute cycles to complete. The speed and efficiency of a computer's processor in executing these cycles determine how quickly the task is finished.


### [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)

1. What is Elastic Beanstalk?
   * Elastic Beanstalk is a fully managed platform-as-a-service (PaaS) offered by Amazon Web Services (AWS). It provides a high-level abstraction layer for deploying and managing applications in the AWS cloud, allowing developers to focus on writing code rather than managing the underlying infrastructure. Elastic Beanstalk supports popular programming languages and frameworks, providing an easy and streamlined way to deploy, scale, and update applications.

2. Describe the relationship between EC2 and Elastic Beanstalk.
   * EC2 and Elastic Beanstalk are closely related, as Elastic Beanstalk leverages EC2 instances to host the application environment. Elastic Beanstalk manages the underlying EC2 instances, along with other AWS resources such as load balancers, auto-scaling groups, and storage. When deploying an application using Elastic Beanstalk, it provisions and manages the necessary EC2 instances, networking, and storage infrastructure automatically. EC2 instances are used by Elastic Beanstalk to run the actual application code and handle incoming requests.
  
3. Name some benefits of using Elastic Beanstalk.
  a. Elastic Beanstalk simplifies deployment by automating infrastructure setup, provisioning EC2 instances, load balancing, and auto-scaling.
  b. Elastic Beanstalk enables automatic scalability and high availability by dynamically scaling the application based on traffic demands and distributing requests across multiple EC2 instances.
  c. Elastic Beanstalk integrates with AWS CloudWatch for comprehensive application monitoring, providing detailed metrics, logs, and health checks to ensure smooth performance.
  d. Elastic Beanstalk supports a wide range of programming languages, frameworks, and platforms, making it easy to deploy applications built with different technologies.
  e. Elastic Beanstalk facilitates easy updates and rollbacks of application versions, tracking multiple versions for seamless deployment management.
  f. Elastic Beanstalk seamlessly integrates with various AWS services, including Amazon RDS, Amazon S3, and Amazon VPC, allowing you to leverage additional services within your application environment.

## Bookmark and Review

[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)