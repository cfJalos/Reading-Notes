# Reading 3: Data Modeling & NoSQL Databases

## Reading, Research, and Discussion

**1. Why would a developer choose to make data models?**

Models are essentially constructors that use schema to create instances of documents, much like you would with a record in a relational database. A developer might choose to make data models in order to regulate the "shape" of data being stored in the database, or to take large amounts of disparate data and convert it into standardized instances of documents.

**2. What purpose do CRUD operations serve?**

"CRUD" stands for "Create, Read, Update, and Delete" - the four basic types of functionality for peristent storage. Create, Read, Update, and Delete are standard database commands that are the basis of this paradigm. If an application or model is able to perform all of these actions, it is considered "full CRUD" - meaning that, essentially, CRUD operations serve as the basis for a "complete" application.

CRUD operations allow interactions with persistent storage - Creating/storing data (Create), accessing data (Read), updating data with new information (Update), and deleting data (Delete). Essentially, the full cycle of how a user might expect to interact with data in a fully-fledged application.

**3. What kind of database is Postgres? What kind of database is MongoDB?**

**Postgres is a Relational Database - which uses SQL.**

Relational (SQL) databases are based off of tables, and represent data as tables with a certain number of columns and rows of data. They use schemas to determine and define how data must be composed when inserted.

**MongoDB is a non-relational or distributed database - which is a non-SQL database (NoSQL).**

Non-Relational (NoSQL) databases are based off of documents, key-value pairs, graphs, wide-column stores, or other irregular data. The database consists of two or more files in different sites, and may be stored across multiple computers or networks.

NoSQL databases are a collection of data (can be in the forms previously listed) that do not have a standard schema definition. They allow for the storage and manipulation of unstructured, semistructured, or irregularly-structured data. Schemas are optional.

**4. What is Mongoose and why do we need it?**

Mongoose is an Object Data Modeling (ODM) library designed for use with MongoDB and Node. It helps make manipulating data via MongoDB much easier, as it manages the relationships between the data, constructs/validates schema, and translates objects seamlessly between MongoDB and actual code to make them easier to understand. Ultimately, Mongoose makes working with MongoDB much simpler and familiar due to its numerous features and utilities for modeling data and data relationships.

**5. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.**

In a personal library application with a persistent database, there could be the following pieces of related data:

- Books
- Authors
- User Collection

Each Book has an Author. Each Book can also be saved by the user in a Collection of their choosing - perhaps organized by genre or category. A Book may be saved into multiple collections (one-to-many relationship). Authors are not related directly to the Collection a Book is stored in.

## Vocabulary Terms

- `database`: An organized collection of data/information stored electronically in a computer system, and controlled/accessed via a Database Management System (DBMS).[Source](https://www.oracle.com/database/what-is-database.html).

- `data model`: A data structure that determines how data is organized, as well as how its elements relate to one another. [Source](https://cedar.princeton.edu/understanding-data/what-data-model).

- `CRUD`: An acronym for the four basic SQL commands: Create, Read, Update, and Delete. Each corresponds to an HTTP method. Most modern applications feature some or full CRUD functionality. "CRUD applications" use forms to access information in a database. [Source](https://docs.jboss.org/tools/3.3.0.Final/en/seam_tools_ref_guide/html/crud_database_application.html#:~:text=CRUD%20is%20an%20acronym%20for,and%20out%20of%20a%20database.).

- `schema`: A collection of data structures that determines how data can be inserted into a database. Lays out the structure and organization of a database.[Source](https://database.guide/what-is-a-database-schema/).

- `unit test`: A test that runs in isolation - focusing on a single block of code or individual module. [Source]().

- `sanitize`: The process of checking data to ensure there are no inputs that might make the program vulnerable to attacks (such as a SQL injection attack). Prevents users from entering data directly into a database. [Source]().

- `Structured Query Language (SQL)`: A standard language used to access and manipulate databases through the use of queries and commands. Multiple versions of the language exist, all with standard commands. [Source](https://www.w3schools.com/sql/sql_intro.asp).

- `Non SQL (NoSQL)`: NoSQL databases have dynamic schema for unstructured data. Popular with more complex web applications.[Source](https://www.oracle.com/database/what-is-database.html).

- `MongoDB`: A cross-platform, document-oriented, NoSQL database program (non-relational/distributed database). Utilizes documents with a JSON-style format. Schemas are optional. [Source](https://en.wikipedia.org/wiki/MongoDB).

- `Mongoose`: An Object Data Modeling (ODM) library built for MongoDB and Node.js. Manages relationships between data, validates schema, and translates objects between code and their format in MongoDB. [Source](https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/).

- `record`: An object representing a group of data saved in a database table. Displays a set of fields related to the object's properties and values (such as an employee ID, name, position, hire date, etc.). [Source](https://teachcomputerscience.com/database-record/).

- `document`: A JSON-like model for storing irregular data in a database. Map to objects in code for a more natural/intuitive flow. [Source](https://www.mongodb.com/document-databases).

- `Object Relation Mapping (ORM)`: A layer laid over the top of Relational Databases that helps to make data more readable in a non-SQL format.