# Reading

## SQL

> SQL, short for Structured Query Language, is a programming language designed for managing and manipulating relational databases. It provides a standardized way to interact with databases, allowing users to create, retrieve, update, and delete data.

## NOSQL

> NoSQL, or "Not Only SQL," is a term used to refer to non-relational databases that provide flexible data models for storage and retrieval of data. Unlike traditional SQL databases, NoSQL databases do not use a fixed schema and are designed to handle large volumes of unstructured or semi-structured data.

---

### What type of database is the best fit for the complex query intensive environment?

For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.
[link](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

### What type of database is the best fit for hierarchical data storage?

For the type of data to be stored: SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data)

### Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

- In a **SQL** database, scaling can be like adding more shelves to accommodate more items. It can become complicated and time-consuming as the database grows.

- In a **NoSQL** database, scaling is like using flexible containers. You can easily add more containers to store more items as your database expands. It's simpler and faster to scale up.

---

## Data Modeling Concepts

### Among data tables, what is a one-to-many relationship and how do we “relate” them?

We connect lines between tables to show relationships. In some cases an entry in one table can be related to more than one entry in another. This is called a one-to-many relationship. In our example there are many employees in on department; therefore, we show a many-to-one relationship.

### Prior to designing your relational database, it might be useful to *diagram* a *create* of the database tables and their relationships.

---

### Explain the difference between a primary and foreign key.

A primary key is like a unique identification number for each record in a table. It ensures that each record has a distinct identity and can be uniquely identified. It is like a person's National Number (ID) . The primary key is used to enforce data integrity and provide a quick way to look up specific records.

A foreign key, on the other hand, is like a reference to a primary key in another table. It establishes a relationship between two tables. It's similar to a cross-reference between different documents. A foreign key in one table refers to the primary key in another table, creating a connection between them. This connection helps maintain data consistency and enables queries that retrieve related data from multiple tables.

> In short, a primary key uniquely identifies a record within a table, while a foreign key establishes a relationship between tables by referring to the primary key in another table.

---

### How do we treat keywords and parameters differently in SQL syntax?

Keywords in SQL have predefined meanings and are crucial for defining the structure and actions of SQL statements. Examples of these keywords include `SELECT`, `INSERT`, `UPDATE`, `DELETE`, and `CREATE`. They fundamental in specifying the operations to be performed on the database, such as retrieving data, inserting records, updating existing data, deleting records, and creating database objects.


### Define normalization within the context of schemas and data? 

Normalization ensures that data is organized in a way that fits the table structure. It minimizes redundancy and improves data storage and retrieval. 

### Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.


- **One-to-One Relationship:**
Two entities have a one-to-one relationship when each entity is associated with only one instance of the other entity.

- **One-to-Many Relationship**
Two entities have a one-to-many relationship when one entity is associated with multiple instances of the other entity, but each instance of the other entity is associated with only one instance of the first entity.

- **Many-to-Many Relationship**
Two entities have a many-to-many relationship when multiple instances of each entity are associated with multiple instances of the other entity.
