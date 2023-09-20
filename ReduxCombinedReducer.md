# Readings: Redux - Combined Reducers


## Why create multiple reducers?

In Redux, multiple reducers are employed to manage different aspects of an application's state separately. This approach enhances code modularity and maintainability.

### How would you combine multiple reducers?

To combine multiple reducers, Redux provides the `combineReducers` utility, which creates a single state tree from individual reducers.

### How will you manage state as an immutable object? why?

Redux promotes treating state as immutable to ensure predictability and simplify debugging.

### `combineReducers` 

`combineReducers` takes state slices and their corresponding reducers, consolidating them into a unified state tree.

### How would you define initial state in an app using `combineReducers`?

You can specify the initial state using `combineReducers` by supplying an initial state object that matches the structure of the state slices managed by individual reducers.

### Why will you want to split your reducing functions as your app becomes more complex?


In complex applications, it's advisable to split reducers to maintain a clear and organized code structure. This allows you to focus on specific state portions and their respective logic, simplifying debugging, testing, and scalability.

### Reducer Naming Convention

A widely used convention for naming reducers is to choose descriptive names that indicate the managed state slice. For example, a reducer handling user data might be named `userReducer`. This naming convention aids in quickly understanding the purpose of each reducer in a large application.
