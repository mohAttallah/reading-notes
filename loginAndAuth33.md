## Reading: `<Login />`and `<Auth />`

### Role-based access control (RBAC)

restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties.


### example of RBAC including all possible CRUD operations and correlating roles

RBAC allows precise control of user permissions based on their roles. It classifies users (administrators, specialists, end-users) and aligns their access accordingly. Key components include Management Role Scope, Role Group, Role, and Role Assignment. Users in a group get access to all roles; removal restricts access. Additional access options include Primary, Billing, Technical, and Administrative roles.



- **Management Role Scope**: Limits the objects a role group can manage.

 - **Management Role Group**: Allows for the addition and removal of members.

- **Management Role**: Specifies the tasks a role group can perform.

- **Management Role Assignment**: Links a role to a role group.

### RBAC offers several key benefits:

1- **Enhanced Security:** It ensures that access to sensitive information is strictly based on each user's role, reducing the risk of unauthorized access.

2- **Efficiency:** RBAC simplifies user management, minimizing administrative work and IT support by quickly adding or changing roles across systems and applications, reducing errors.

3- **Operational Efficiency:** It aligns roles with the organizational structure, enabling users to work more efficiently and independently.

4- **Compliance:** RBAC helps organizations meet statutory and regulatory requirements for data privacy and confidentiality, particularly in sectors like healthcare and finance with sensitive data handling.

 RBAC improves security, streamlines operations, and aids in compliance, offering significant benefits to organizations.



### Compare and Contrast between (react-cookie library, react-cookies component)

**react-cookie** library:

- Features: 
  - Manage cookies in React applications.
  - Set, get, and delete cookies.
  
**react-cookies** component:

- Features:
  - Simplified reading and writing of cookies.
  - Focused on rendering cookie-related content.
  
**Preference:**

- If you need comprehensive cookie management within your React application, prefer **react-cookie**.

- If you prefer a simplified approach for reading and writing cookies, and your main focus is on rendering cookie-related content, consider **react-cookies**.

Choose the library or component that best fits your project's requirements.
