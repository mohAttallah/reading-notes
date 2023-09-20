# Readings: Redux - Asynchronous Actions

## Why should we consider using Redux middleware?
Redux middleware is used to manage tasks like fetching data and logging in an organized manner, acting as a bridge between user actions and data updates.

## Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.
In Redux's async flow, user actions trigger messages (dispatch actions) that pass through middleware for tasks like data fetching. Real actions are dispatched afterward, updating the app's state and interface.


## How are we accommodating async in our Redux app?
Redux uses Thunk middleware to handle asynchronous tasks efficiently, allowing you to create specialized action creators for these tasks.

## Why would you need `redux-thunk` middleware?

Redux-thunk is crucial for managing async operations in Redux, as it enables you to write action creators for tasks like API requests.

### Redux Thunk middleware allows you to write action creators that return a ____ instead of an action

- Function 