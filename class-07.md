[Home page](https://cfjalos.github.io/code201-reading-notes/)

# Object-Oriented Programming, HTML Tables # 

## What's a table? ##

* A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

* Grades allow us to understand complex data by referencing information to access.

* Each block in the grade is your fair to us a table. In HTML the table is written in a row by row.

```html
<table> - element represents tabular data — that is, information presented in a two-dimensional table comprised of rows and columns of cells containing data.

<tr> element defines a row of cells in a table. The row's cells can then be established using a mix of <td> (data cell) and <th> (header cell) elements.

<thead> element defines a set of rows defining the head of the columns of the table.

<th> element defines a cell as header of a group of table cells. The exact nature of this group is defined by the scope and headers attributes.

Table Body element (<tbody>) encapsulates a set of table rows (<tr> elements), indicating that they comprise the body of the table (<table>).

<td> element defines a cell of a table that contains data. It participates in the table model.

<tfoot> element defines a set of rows summarizing the columns of the table.
```


## Object-Oriented Programming ##

* Object constructor creates an object wrapper for the given value.

* Arrays are actually a special type of object. They hold a related set of key/pairs value like all objects, but the key for each value is its index number.

* You can combine arrays and objects to create complex data structures.

  * Arrays can store a series of objects.

  * Objects can also hold arrays.

### Global Object ##

* A global object is an object that always exists in the global scope.

* objects can be seen as a collection of properties. With the object literal syntax, a limited set of properties are initialized; then properties can be added and removed. Property values can be values of any type, including other objects, which enables building complex data structures. Properties are identified using key values. A key value is either a String or a Symbol value.

**Six Data types**

* Six Data Types 

  * undefined : typeof instance === "undefined"
  * Boolean : typeof instance === "boolean"
  * Number : typeof instance === "number"
  * String : typeof instance === "string"
  * BigInt : typeof instance === "bigint"
  * Symbol : typeof instance === "symbol"