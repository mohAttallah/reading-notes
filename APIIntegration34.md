# API Integration

### Explain the different between a query string parameter and a path parameter.

**Query String Parameter:**

- **Location:** Query string parameters are typically located in the URL after a question mark (`?`) and separated by ampersands (`&`) or slashes (`/`).

- **Purpose:** Query string parameters are used to send additional data to a server when making an HTTP request. They are commonly used in GET requests to filter, sort, or specify information related to the request.

- **Visibility:** Query string parameters are visible to users as they appear in the URL. Users can modify them, but they don't affect the structure of the URL path.

- **Example:** In the URL `https://example.com/search?query=apple&page=1`, `query` and `page` are query string parameters, and their values are `apple` and `1`, respectively.

**Path Parameter:**

- **Location:** Path parameters are part of the URL path and are typically enclosed in curly braces `{}`.

- **Purpose:** Path parameters are used to define variables or placeholders within the URL path itself. They often represent resource identifiers or data that is part of the URL's structure.

- **Visibility:** Path parameters are not as visible to users because they are part of the URL path. Users can't easily modify them without changing the structure of the URL.

- **Example:** In the URL `https://example.com/users/{username}/profile`, `{username}` is a path parameter, and its value might be something like `john_doe`, making the complete URL `https://example.com/users/john_doe/profile`.


### What would our API URL with a path id parameter be given the following information:

The API URL with a path id parameter would be:

`http://our-site.com/v3/stuff/things`

In this URL:
- `http://our-site.com` is the domain.
- `v3` represents the API version.
- `stuff` is the model name.
- `things` is the id parameter in the path.

### We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.


We created an interface for our online store's data. It helps our website talk to a big database.

**How it works:**

- **Getting Data:** We can ask for all or specific products and categories.

- **Adding Data:** We can add new products.

- **Updating Data:** We can change product details.

- **Deleting Data:** We can remove products.

- **Rules:** It follows specific web addresses (like `/api/v1/products/12345`) and understands special requests.

- **Language:** It speaks JSON, a universal language.

In a nutshell, it's like a special phone line between our website and the database, making sure everything runs smoothly.


### Describe how you would use middleware to implement basic and bearer auth.

- To implement Basic Auth Middleware, we first validate the user's account in our database. If valid, it returns an object containing a re-authentication/bearer token along with the user object. In case of an error, it returns an error object.

- For OAuth, the process begins in the browser with a 3rd party authentication/authorization service. Once the user grants permission, it triggers a GET request to our /oauth route. The OAuth Middleware then completes the handshaking process, creates or updates a local user account in our database, and returns an object containing a re-authentication/bearer token and the user object.




### Describe the handshake necessary to implement OAuth.
- The OAuth handshake is a secure process where a user grants permission to a third-party app to access their data. It involves user consent, authorization code exchange, and access token issuance, ensuring secure data access without sharing credentials.


### Describe how Role Based Access Control works to a non-technical friend.

Role-Based Access Control (RBAC) is like giving people keys to different rooms in a building:

- Some have keys to all rooms (admins).
- Some have keys to specific rooms (specialists).
- Some have keys to just one room (end-users).

When someone's job changes, we change their key. RBAC keeps things organized, like using keys to open only the right doors in a building.




