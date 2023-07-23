# Reading
## An introduction to NodeJS and Express

**1. Explain middleware, answer as though I were a non-technical recruiter.**
   Middleware is like a series of filters or handlers that intercept requests and responses in an Express application. It helps to modify, validate, or process data before it reaches the final destination. Think of it as a way to add extra functionality to the application without modifying the core code.

**2. Express is the most popular _______ ______.**
   Express is the most popular Node web framework and serves as the underlying library for several other popular Node web frameworks. [Express Node.js introduction on Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction#introducing_express).

**3. Express is "unopinionated." What does that mean?**
   Express is unopinionated. It allows you to insert almost any compatible middleware into the request handling chain in any order you prefer. You have the flexibility to structure your application in one file or multiple files, and you can use any directory structure that suits your needs. With Express, you may sometimes feel overwhelmed by the numerous choices available to you. [Express unopinionated](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction#what_does_express_code_look_like).

**4. What is a module, and why is modularity useful to us as developers?**
A set of functions you want to include in your application,
It allows developers to organize and separate different parts of an application, promoting reusability, scalability, and collaboration. 
[nodejs Moudules](https://www.w3schools.com/nodejs/nodejs_modules.asp)

<!-- https://www.w3schools.com/nodejs/nodejs_modules.asp -->


## NPM

> **What is NPM?**
>
>  NPM stands for Node Package Manager. It is a package manager for Node.js that allows developers to easily install, manage, and share reusable code packages (libraries, frameworks, tools) for their Node.js projects.

**1. What command would you type to install a library/package called 'jshint' into your node project?**
   To install the 'jshint' library/package into your Node project, you can run the following command in your terminal: `npm install jshint`.

**2. What version of npm are you running on your machine?**
   To check the version of npm installed on your machine, you can run the following command in your terminal: `npm -v`.

## TDD

> **What is TDD?**
>
> TDD stands for Test-Driven Development. It is a software development approach where developers write tests before writing the actual code. It helps ensure that the code meets the desired requirements and enables more robust and maintainable software development.


**1. Explain why tests are important. Please explain as though I were your non-technical elder.**
   Tests are important because they help ensure that the software we build works correctly and reliably. They act as a safety net, catching potential issues and bugs before they reach users. By having tests, we can have confidence in the quality of our code and make sure it continues to work as expected even when changes are made.

**2. What are three expected benefits of testing?**
    - Increased code reliability and quality.
    - Faster identification and fixing of bugs.
    - Improved maintainability and scalability of the codebase.

**3. Name at least 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.**
    - Individual pitfalls: Over-testing (writing too many tests for trivial functionality), neglecting edge cases.
    - Team pitfalls: Lack of communication and coordination between team members regarding test coverage, inconsistent or poorly defined testing standards.

## CI/CD
>CI/CD stands for Continuous Integration and Continuous Delivery/Deployment. It is a software development practice that involves automating the process of building, testing, and deploying code changes. In Node.js, CI/CD allows developers to continuously integrate their code changes, run automated tests to ensure quality, and deploy the application to production environments seamlessly. It helps in reducing manual errors, improving collaboration among team members, and delivering software updates more frequently and reliably.
>[The CircleCI Blog](https://circleci.com/blog/what-is-ci-cd/)


**1. What are three benefits of Continuous Integration?**
   - Early detection of integration issues.
   - Faster feedback loop for developers.
   - Improved code quality and stability.

**2. What is the difference between Continuous Delivery and Continuous Deployment?**
   Continuous Delivery (CD) is the practice of ensuring that the code is always in a releasable state, ready to be deployed at any time. Continuous Deployment (CD) takes it a step further and automatically deploys the code to production after passing all the necessary tests.

**3. Explain how GitHub fits into this process assuming the listener comes from a non-technical background.**
   GitHub is a web-based platform that provides version control and collaboration for developers. In the context of CI/CD, GitHub acts as a central repository where developers store their code and collaborate on it. It enables teams to work together, manage code changes, and track issues and features. Continuous Integration systems can integrate with GitHub, automatically triggering builds and tests whenever code changes are pushed to the repository. This ensures that the latest changes are tested and integrated with the existing codebase before being deployed to production.
## Things I want to know more about

how checks are performed on GitHub and how code is read in the context of CI/CD ?