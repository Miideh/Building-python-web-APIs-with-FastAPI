#

Chapter 6 was basically about SQL and NoSQL databases using SQLModel and Beanie, respectively, in our FastAPI application. The goal was to enhance our backend application with robust database support.

SQL Databases with SQLModel:
We started by incorporating SQL databases into our application using SQLModel, which combines the best features of SQLAlchemy and Pydantic. SQLModel provides a convenient way to define SQL tables and perform CRUD operations without losing type safety or code clarity.

Defining Models:
SQL models were created using SQLModel classes, defining attributes and types, and specifying primary keys and relationships.

Setting Up Database Connection:
Database connection was configured using SQLAlchemy's `create_engine` function. This connection is essential for executing SQL commands and managing database sessions.

CRUD Operations:
With the models and connection set up, CRUD operations (Create, Read, Update, Delete) was implemented using SQLModel's session object. T.

NoSQL Databases with Beanie:
Focus was then shifted to NoSQL databases by introducing Beanie, an ODM (Object-Document Mapper) for MongoDB that provides type-safe models and asynchronous operations.

Defining Models:
Similar to SQLModel,NoSQL models were definedusing Beanie's `Document` class, specifying attributes and data types.

Connecting to MongoDB:
A connection was established to the MongoDB server using Motor and configured Beanie to use this connection for managing our documents.

CRUD Operations:
Beanie allowed us to perform CRUD operations with MongoDB documents asynchronously, enhancing the performance and scalability of our application.

Testing Routes:
After integrating SQL and NoSQL databases,focus was shifted to  testing our API routes to ensure they functioned as expected.
