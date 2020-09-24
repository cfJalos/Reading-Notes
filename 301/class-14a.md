# Online Reading

## [Database Normalization Explained in Simple English](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

**Database Normalization Explained in Simple English**

* Introduction to Database Normalization 
  - Database normalization - a process used to organize a database into tables and columns. Main idea is that a table should be about a specific topic with only supporting topics included. 
  - Example: When making a spreadsheet with info on salespeople and customers. First identify salespeople in your organization, then list all customers your company calls upon to sell a product, and finally identify which salespeople call on specific customers. 
  - Limit the table to one purpose to reduce data duplication within a database, and this also eleminates issues with database modification.

* Reasons for Database Normalization
  - 1st to minimize duplicate data
  - 2nd to minimize or avoid data modification issues
  - 3rd to simplify queries
  - In a table that hasn't been normalized, you will notice that it serves many purposes instead of just one purpose, which could cause data duplication, data update issues, and increased effort to query data, as mentioned above.

* Data Duplication and Modification Anomalies
  - Data duplication present two problems: 
    * 1st - it increases storage and decrease performance
    * 2nd - it becomes more difficult to maintain data changes
  - Modification anomalies:
     * Insert anomaly - caused by facts that cannot be recorded until we know information for the entire row
     * Update anomaly - caused by the rows not being updated, which will make inconsistences appear
     * Deletion anomaly - caused by the deletion of a row, which will cause removal of more than one set of facts

* Search and Sort Issues
  - Database normalization makes it easier to search and sort data. So, when you are normalizing a database its best to keep it simple.

* Definition of Database Normalization
  - Three common forms of database normalization, which are abbreviated as 1NF, 2NF, and 3NF.
  - The forms are progressive, which means that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. 
  - First Normal Form (1NF) – the information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
  - Second Normal Form (2NF) – the table is in first normal form and all the columns depend on the table’s primary key.
  - Third Normal Form (3NF) – the table is in second normal form and all of its columns are not transitively dependent on the primary key.