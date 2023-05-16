# Express, NPM, TDD, CI/CD

## [An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

1. Explain middleware, answer as though I were a non-technical recruiter.


Middleware is a software component that acts as a bridge between different applications or systems. It helps in managing and processing data as it travels between these systems. Think of it as a translator or a mediator that facilitates communication and coordination between different parts of a software application. It can handle tasks like authentication, data validation, logging, and error handling, making it easier for different software components to work together seamlessly.

2. Express the most popular __ __ ____.

Express is the most popular Node Web Framework

It is the underlying library for a number of other popular Node web frameworks. It provides mechanisms to:

* Write handlers for requests with different HTTP verbs at different URL paths (routes).
Integrate with "view" rendering engines in order to generate responses by inserting data into templates.

* Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.

* Add additional request processing "middleware" at any point within the request handling pipeline.

3. Express is “unopinionated.” What does that mean?

In the context of Express, being "unopinionated" means that the framework does not enforce strict rules or opinions on how you should structure or organize your application. It gives you the freedom to make architectural decisions and choose from various libraries and tools based on your preferences and project requirements. Express provides a minimalistic and flexible foundation for building web applications, allowing developers to have more control and customization over their code.

4. What is a module and why is modularity useful to us as developers?

A module is a self-contained unit of code that encapsulates related functionality. It allows developers to organize their code into logical and reusable components, making it easier to manage and maintain complex software systems.

Modularity is useful to us as developers for several reasons:

* Reusability: Modules can be reused across different projects, reducing the need to write the same code from scratch. This saves time, effort, and promotes code efficiency.

* Maintainability: By breaking down a large system into smaller modules, each module becomes more manageable and easier to understand. Changes or updates can be made to a specific module without impacting the entire system, making maintenance and debugging more efficient.

* Encapsulation: Modules provide a way to encapsulate related functionality, hiding internal implementation details and exposing only the necessary interfaces. This promotes code organization, improves readability, and helps in creating more maintainable and scalable applications.

* Collaboration: Modularity enables developers to work on different modules simultaneously without interfering with each other's work. This promotes parallel development and collaboration within a team, increasing productivity.

* Testing: Modules can be individually tested, making it easier to isolate and verify the functionality of specific components. This leads to better test coverage and more reliable software.

Overall, modularity improves code organization, reusability, maintainability, collaboration, and testing, which are all essential for efficient software development.

## [What is NPM?](https://docs.npmjs.com/about-npm)

1. What version of npm are you running on your machine?

I am currently running version 9.6.6

2. What command would you type to install a library/package called ‘jshint’ into your node project?

```
npm install jshint
```

## [What is TDD?](https://www.agilealliance.org/glossary/tdd/)

1. Explain why tests are important. Please explain as though I were your non technical elder.

Tests are important because they help us catch mistakes early, ensure our software works as intended, and maintain its quality over time. They provide reassurance, promote collaboration, and help us make changes confidently.

2. What are three expected benefits of testing

* Bug Detection: Testing helps in identifying bugs, errors, and issues in the software early in the development process. By running tests, we can catch and fix these problems before they affect end-users, resulting in more stable and reliable software.

* Quality Assurance: Testing ensures that the software meets the expected requirements and performs as intended. It helps validate that the functionality and behavior of the software align with the desired specifications, improving overall quality and user satisfaction.

* Maintenance and Refactoring: Testing provides a safety net when making changes or adding new features to the software. By having tests in place, we can verify that existing functionality remains intact, preventing regressions and enabling developers to refactor code with confidence. This leads to more maintainable and scalable software systems.

3. Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.


## [CI/CD](https://www.youtube.com/watch?v=xSv_m3KhUO8)

1. What are three benefits of Continuous Integration?

### Individual pitfalls commonly encountered while writing tests include:

Over-reliance on Happy Path Testing: Focusing only on testing the expected or ideal scenarios is known as the "happy path." This can lead to insufficient coverage of edge cases, error handling, and boundary conditions, leaving potential issues undetected.

Lack of Test Maintainability: Tests should be easy to understand, maintain, and update as the software evolves. A pitfall is writing tests that are overly complex, tightly coupled to implementation details, or difficult to modify. This can result in tests becoming a burden to maintain and hinder the agility of development.

### Team pitfalls commonly encountered while writing tests include:

Lack of Test Coverage Agreement: Teams may face challenges in deciding and aligning on the appropriate level of test coverage. If not addressed, it can lead to inconsistent testing practices, gaps in coverage, or excessive duplication of effort.

Insufficient Collaboration and Communication: Lack of collaboration and communication among team members can result in inconsistent testing approaches, redundant or conflicting tests, and difficulties in maintaining a shared understanding of the testing strategy. This can impact the overall effectiveness and efficiency of testing efforts.


2. What is the difference between Continuos Delivery and Continuous Deployment?

Continuous Delivery (CD): Continuous Delivery is an approach where software is continuously built, tested, and prepared for deployment. The focus is on automating the delivery pipeline to ensure that the software is in a releasable state at any given time. With Continuous Delivery, the software can be deployed to production manually at the discretion of the development team or stakeholders. It emphasizes maintaining a high level of quality through rigorous testing and automation, enabling faster and more reliable software releases.

Continuous Deployment (CDep): Continuous Deployment takes the concept of Continuous Delivery further by automating the release process itself. In Continuous Deployment, once changes pass all the necessary tests and quality checks in the delivery pipeline, they are automatically deployed to production without human intervention. The goal is to make the release process completely automated and eliminate any delays or potential errors introduced by manual deployments. Continuous Deployment enables a continuous flow of updates, with new features and bug fixes being quickly and automatically deployed to end-users.

Continuous Delivery focuses on automating the process of preparing software for release, while Continuous Deployment takes it a step further by automating the actual deployment of software changes to production. Both practices aim to increase speed, efficiency, and reliability in software delivery, but Continuous Deployment achieves a higher level of automation and immediate deployment of changes to production.

3. Explain how GitHub fits into this process assuming the listener comes from a non-technical background


GitHub is a platform that helps developers store and manage their code. It supports collaboration and version control, allowing multiple developers to work on the same project simultaneously. With automated tools, it enables continuous integration, testing, and deployment. GitHub also provides features for issue tracking and project management. It promotes transparency, collaboration, and automation in the software development process.