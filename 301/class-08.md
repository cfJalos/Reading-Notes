# Online Readings

## [Complete SQLBolt (Intro, Lessons 1-4, 13-18)](http://sqlbolt.com/)
**Introduction to SQL**
* SQL(Structured Query Language) - is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. 
* Relational database - represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
* SQL goal is to learn how to answer specific questions about data, and make better decisions about it.

* SQL Lesson 1: SELECT queries 101
  - To retrieve data from a SQL database, we need to write SELECT statements, which are refered to as queries. A query is just a statement which declares what data we are looking for, where to find it in the database, and how to transform it before it is returned. 
  - Table in SQL is a type of entity.
  - Columns represent the common properties shared by all instances of that entity.
  - The most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances). 
  - Exercise 1 Task Answers:
    1. SELECT title FROM movies;
    2. SELECT director FROM movies; 
    3. SELECT title, director FROM movies;
    4. SELECT title, year FROM movies;
    5. SELECT * FROM movies;

* SQL Lesson 2: Queries with constraints (Pt. 1)
  - WHERE clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not. More complex clauses can be constructed by joining numerous AND or OR logical keywords. 
  - Write SQL keywords all capitalized.
  - Exercise 2 Task Answers:
    1. SELECT id, title FROM movies 
       WHERE id = 6;
    2. SELECT title, year FROM movies
       WHERE year BETWEEN 2000 AND 2010;
    3. SELECT title, year FROM movies
       WHERE year NOT BETWEEN 2000 AND 2010; 
    4. SELECT title, year FROM movies
       WHERE year <= 2003;

* SQL Lesson 3: Queries with constraints (Pt. 2)
  - When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching.
  - All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.
    - Exercise 3 Task Answers:
    1. SELECT title, director FROM movies 
       WHERE title LIKE "Toy Story%";
    2. SELECT title, director FROM movies 
       WHERE director = "John Lasseter";
    3. SELECT title, director FROM movies 
       WHERE director != "John Lasseter"; 
    4. SELECT * FROM movies 
       WHERE title LIKE "WALL-_";

* SQL Lesson 4: Filtering and sorting Query results
  - DISTINCT keyword - way to discard rows that have a duplicate column value.
  - GROUP BY clause - discard duplicates based on specific columns using grouping.
  - ORDER BY clause - provides a way to sort your results by a given column in ascending or descending order. When specified, each row is sorted alpha-numerically based on the specified column's value.
  - LIMIT and OFFSET clauses - LIMIT will reduce the number of rows to return, and OFFSET will specify where to begin counting the number rows from. Applied last.
     - Exercise 4 Task Answers:
    1. SELECT DISTINCT director FROM movies
       ORDER BY director ASC;
    2. SELECT title, year FROM movies
       ORDER BY year DESC
       LIMIT 4; 
    3. SELECT title FROM movies
       ORDER BY title ASC
       LIMIT 5;
    4. SELECT title FROM movies
       ORDER BY title ASC
       LIMIT 5 OFFSET 5;

* SQL Lesson 13: Inserting rows
  - Database schema is what describes the structure of each table, and the datatypes that each column of the table can contain. Example:  in our Movies table, the values in the Year column must be an Integer, and the values in the Title column must be a String. This fixed structure is what allows a database to be efficient, and consistent despite storing millions or even billions of rows.
  - INSERT statement - used to insert data into database. Declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.
  - Exercise 13 Task Answers:
    1. INSERT INTO movies VALUES (4, "Toy Story 4", "El Directore", 2015, 90);
    2. INSERT INTO boxoffice VALUES (4, 8.7, 340000000, 270000000); 

* SQL Lesson 14: Updating rows
  - UPDATE statement - to update existing data, and has to match the data type of the columns in the table schema. Where clause needs to be included.
  - Always write the constraint first and test it in a SELECT query to make sure you are updating the right rows, and then writing the column/value pairs to update.
  - Exercise 14 Task Answers:
    1. UPDATE movies
       SET director = "John Lasseter"
       WHERE id = 2;
    2. UPDATE movies
       SET year = 1999
       WHERE id = 3;
    3. UPDATE movies
       SET title = "Toy Story 3", director = "Lee Unkrich"
       WHERE id = 11; 

* SQL Lesson 15: Deleting rows
  - DELETE statement - use this to delete data from a table in the database.
  - Example: DELETE FROM mytable
             WHERE condition;
  - Run the constraint in a SELECT query first to ensure that you are removing the right rows. Without a proper backup or test database, it is downright easy to irrevocably remove data, so always read your DELETE statements twice and execute once.
  - Exercise 15 Task Answers:
    1. DELETE FROM movies
       where year < 2005;
    2. DELETE FROM movies
       where director = "Andrew Stanton";

* SQL Lesson 16: Creating tables
  - CREATE TABLE statement - used to create new database table. Example: 
  CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
   );
  - The structure of the new table is defined by its table schema, which defines a series of columns. Each column has a name, the type of data allowed in that column, an optional table constraint on values being inserted, and an optional default value.
  - IF NOT EXISTS clause - can use this to suppress the error and skip creating a table if one exists.
  - Table data types - INTEGER, BOOLEAN, FLOAT, DOUBLE, REAL, CHARACTER(num_chars), VARCHAR(num_chars), TEXT, DATE, DATETIME, and BLOB
  - Table constraints -  each column can have additional table constraints on it which limit what values can be inserted into that column. Constraints: PRIMARY KEY, AUTOINCREMENT, UNIQUE, NOT NULL, CHECK, and FOREIGN KEY
  - Exercise 16 Task Answer:
    1. CREATE TABLE Database (
       Name TEXT,
       Version FLOAT,
       Download_count INTEGER
     );

* SQL Lesson 17: Altering tables
  - ALTER TABLE statement - a way for you to update your corresponding tables and database schemas, and to add, remove, or modify columns and table constraints.
  - FIRST or AFTER clauses - used to specify where to insert the new column.
  - Removing columns: ALTER TABLE mytable
                      DROP column_to_be_deleted;
  - Renaming the table - to rename the table use RENAME TO clause.
  - Exercise 17 Task Answers:
    1. ALTER TABLE Movies
       ADD COLUMN Aspect_ratio FLOAT DEFAULT 2.39;
    2. ALTER TABLE Movies
       ADD COLUMN Language TEXT DEFAULT "English";

* SQL Lesson 18: Dropping tables
  - DROP TABLE statement - use this to remove an entire table including all of its data and metadata. Statement: DROP TABLE IF EXISTS mytable;
  - Use the IF EXISTS clause when the database may throw an error if the specified table does not exist, and to suppress that error.
  - Exercise 17 Task Answers:
    1. DROP TABLE Movies;
    2. DROP TABLE BoxOffice;

## [W3 Schools](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)
* Resource that can be used to practice writting SQL queries, and practice examples.

# Additional Resources
## [A Primer on SQL](https://openlibra.com/en/book/a-primer-on-sql-3rd-edition)

**Introduction to SQL(Structured Query Language)**
* Database - a collection of organized data
* Database Management System (DBMS) - Software which is used to manage a digital database.
* Relational Model -  data to be stored is organized as rows inside a table with the column headings
specifying the corresponding type of data stored. 
* Relation - a mathematical term that is roughly equivalent to a table itself.
* SQL(Structured Query Language) - de-facto standard for interacting with relational databases.
* SQL Commands Classification: 
  - Data Definition Language (DDL) : CREATE TABLE, ALTER TABLE, DROP TABLE etc. These commands allow you to create or modify your database structure.
  - Data Manipulation Language (DML) : INSERT, UPDATE, DELETE. These commands are used to manipulate data stored inside your database.
  - Data Query Language (DQL) : SELECT. Used for querying or selecting a subset of data from a database.
  - Data Control Language (DCL) : GRANT, REVOKE etc.
    Used for controlling access to data within a database, commonly used for granting user privileges.
  - Transaction Control Commands : COMMIT, ROLLBACK etc. Used for managing groups of statements as a unit of work.
* Table - a matrix of data where the columns describe the type of data and the row contains the actual data to be stored. 
* Field - a column in a database
* Record - a row
* Primary key - the id field serves as a good primary key.
* Getting your database ready can be done by using ingres, SQLite, or creating your own database.
* Command createdb is used to create a database.
* Table creation using the command CREATE TABLE
* Inserting data - command INSERT
* Example of simple query: SELECT Selection FROM Table Name;
* Constraints - a rule that you apply or abide by while doing SQL operations.
* Primary key - used to make each record unique in atleast one way by forcing a field to have
unique values. A primary key field cannot take on a NULL value, whereas a field with a unique constraint
can. You are allowed to define only one primary key constraint but you can apply the unique
constraint to as many fields as you like.
* Unique key - used to make each record inside a table unique.
* Dropping Tables - use DROP TABLE command
* Creating new tables from existing tables - syntax: CREATE TABLE New Table AS SELECT Selection FROM Old Table;
* Modifying tables - use ALTER TABLE command
* Query - a SQL statement that is used to extract a subset of data from your database and presents
it in a readable format. 
* Ordering results - with ORDER BY clause
* WHERE clause - used to limit the number of records retrieved in a query using conditions. 
* Combining conditions - using boolean operators AND, OR
* NULL - null values in statements like INSERT.
* UPDATE command - To modify some data in a record
* DELETE command - to delete records from a table.
* Normalization - process of breaking down a raw database into logical tables and removing redundancies.
* COUNT - used to find out how many records exist in a table without actually outputting the entire contents of these records.
* Column Aliases - lets you rename column headings in the resultant output.
* Aggregate function - used to compute summarization information from a table or tables. 
* MIN function - looks at a particular set of rows and finds the minimum value of the column which is provided as an argument to it.
* GROUP BY clause - used to group records based upon their field values. This clause is placed after the WHERE conditional. 
* HAVING clause places conditions on the groups created by GROUP BY. It must be placed immediately after the GROUP BY, but before the ORDER BY clause.
* Join operation - allows you to retrieve data from multiple tables in a single SELECT query. 
* Subqueries - is a query written as a part of a bigger statement. 


## [SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)

**SQL Cheat Sheet**

* A quick cheat sheet for SQL(Structured Query Language) on one page.
* Includes:
  - Database Manipulation
  - Table Manipulation
  - Index Manipulation
  - Data Manipulation
  - Select
  - Alias
  - Join
  - Union
  - Select into/in 
  - Create view