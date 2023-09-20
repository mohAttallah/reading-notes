## Redux - Additional Topics


#### **What concerns are addressed by Redux Toolkit?**

- Configuring a Redux store is too complicated
- Add a lot of Packages to get Redux to do anything useful
- Redux requires too much boilerplate code

#### **configureStore()**

wraps `createStore` to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes `redux-thunk` by default, and enables use of the Redux DevTools Extension.


#### **createSlice()**

A function that accepts an initial state, an object of reducer functions, and a `"slice name"`, and automatically generates action creators and action types that correspond to the reducers and state.

#### **Mobx**

MobX is a state management library  that simplifies managing and reacting to changes in your app's state. It revolves around three main concepts:

- Observables: These are your state variables that you want to track.

- Actions: Functions that modify observables.

- Reactions: Functions or components that automatically update when observables change.

#### **How does MobX make it “impossible” to produce an inconsistent state?**


By controlling how state changes (only through actions) and ensuring that reactions update automatically when dependencies change, MobX eliminates the possibility of inconsistent states. This strict system prevents race conditions and ensures predictable and reliable state management in your application.


#### **How would we build a reactive user interface?**
- Design Components: Create reusable UI components and identify their needed data.

- Bind Data: Connect UI elements to state or data properties.

- Handle Events: Implement event handling to update state on user interactions.

- Reactivity: Ensure automatic updates in response to state changes.

- Testing and Optimization: Thoroughly test and optimize for performance.

- Scaling: Organize efficiently for larger applications.



#### **What take-away(s) did this tutorial provide?**
- Using Redux Toolkit: RTK Usage Guide: Explains standard usage patterns for each of Redux Toolkit's APIs
