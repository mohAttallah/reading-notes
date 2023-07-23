# Reading

## ES6

ES6 classes matter because they provide a structured way to work with object-oriented programming in JavaScript. They promote code reusability, encapsulation, and better organization.

**1. Classes are a template for creating objects.**

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are unique to classes. [Classes MND](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes).

**2. Can a class declaration be hoisted?**
No, class declarations have the same temporal dead zone restrictions as let or const and behave as if they are not hoisted. [MND Defining classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes#defining_classes).

**3. How would you describe a constructor and contextual "this" to a non-technical friend?**
- A constructor is like a blueprint for creating something, just like a house blueprint guides the construction of a house.
- In JavaScript, a constructor is a special function that helps create objects based on this blueprint.
- It sets up the initial state and behavior of the object.
- Think of it as a factory that produces objects with predefined properties and methods.

## Routing
Routing is important in JavaScript because it allows us to create dynamic and interactive web applications with multiple pages or views. It enables navigation between different sections of a website without the need for full page reloads.

**1. Within Express, what does routing refer to?**
Routing refers to how an application's endpoints (URIs) respond to client requests. [Routing](https://expressjs.com/en/guide/routing.html)

**2. What is the difference between a route path and a route method?**
- Path: Defines the URL pattern or path that a user can visit to access a specific page or endpoint.
- Route: Represents the action or operation to be performed on a resource identified by the route path.

**3. When is it appropriate to add `next` as a parameter to a route handler and what must you do if 'next' has been passed to your middleware as a parameter?**
It is appropriate to add `next` as a parameter to a route handler when you want to pass control to the next middleware or route handler. If `next` has been passed to your middleware as a parameter, you must invoke `next('route')` to bypass the remaining route callbacks. You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there's no reason to proceed with the current route. [Route handlers](https://expressjs.com/en/guide/routing.html)

## Express Router

**1. What is an Express Router?**
It is a mini express application without all the bells and whistles of an express application, just the routing stuff. Let's take a look at exactly what this means. We'll go through each section of our site and use different features of the Router. [Express Router](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4#express-router)

**2. By what mean do we initialize `express.Router()` in an express server?**
`const router = express.Router()`

**3. What do we use route middleware for?**
Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user. [Router Middleware](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4#route-middleware-router-use)

---

## What are your learning goals after reading and reviewing the class README?
Develop my skills in creating a strong middleware, with Route

## Things I want to know more about
I desperately need to understand how things are going with the `next`
