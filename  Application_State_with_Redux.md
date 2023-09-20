# Application State with Redux

### Principles of Redux

The principles of Redux aren't new, but they are packaged and presented for you in an easy to use a library that not only elevates your applications but also improves your general understanding of building JavaScript UIs.

### Store  

the **store** is the central container for the application's state. It holds the current state, allows access via `getState()`, updates state through `dispatch(action)`, and notifies listeners of changes via `subscribe(listener)`.

**Actions** are plain objects describing state changes. They have a `type` property and optional data (payload).


### createStore  methods 

#### `getState()`
Retrieves the current state of the Redux store, representing your application's data.

#### `dispatch(action)`

Dispatches actions to trigger state changes in the store. Actions describe what should happen in your application.

#### `subscribe(listener)`
 Adds listeners to react to state changes in the store, allowing you to update your UI or perform other actions in response to these changes.


### combineReducers()
combineReducers() in Redux is a tool that helps organize and manage different pieces of the application's state by combining smaller, focused state management functions into one cohesive structure. It's useful for maintaining code clarity, scalability, and collaboration among developers as the application grows.




