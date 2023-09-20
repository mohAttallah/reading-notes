##Context API

The Context API in React allows to share data across components without prop drilling. You create a context, provide data with a Provider, and consume it with `useContext` or a Consumer. It's a convenient way to manage and share state globally in your React application.

####1- **Summarize the five principles for structuring state.**

 -  **Group related state**
        Bundle similar data together for efficient and organized state management.

-   **Avoid Contradictions in State**
        Ensure that application's state remains consistent and doesn't contain conflicting or contradictory information.

-   **Prevent Redundant State**
         Eliminate unnecessary duplication of data in your state to keep it lean and efficient.
-   **Minimize State Duplication**
        Keep the same data in a single place in  state to prevent redundancy and make it easier to update consistently.

-   **Simplify State Nesting**
        keep the state structure as flat as possible to make it more straightforward to access and update specific pieces of data. Avoid unnecessary nesting to reduce complexity.

#### 2- What problem do Contexts aim to solve?
"context" helps solve the problem of efficiently passing data through the component tree by providing a way to share data without the need for excessive prop passing.

#### 3- What is one technique to try before useContext?

**prop drilling**,where you pass data through intermediate components as props. 

#### What hook complements useContext for complex applications?

**useReducer** complements useContext for complex React applications by providing a structured way to manage and update shared state through a predictable reducer function.
