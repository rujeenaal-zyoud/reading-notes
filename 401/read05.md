# Data Modeling
-------------------------------------------------------
#### Three advantages to Test Driven Development

1. Better program design and higher code quality.
2. Detailed project documentation.
3. TDD reduces the time required for project development.
----------------------------------------------
#### what case would you need to use beforeEach() and afterEach() in a test suite?
------------------------------------------------------
**While testing a logger middleware.**

### one downside of Test Driven Development
* Big time investment.

--------------------------------------------------

## The primary difference between ES6 Classes and Constructor/Prototype Classes

*The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.*

*A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.*


------------------------------------------------
#### Why REST ?
1. REST is Easy to Understand and Implement.
2. REST Makes your Application More Scalable.
3. Caching is Easier with REST.
5. REST is Flexibile.
---------------------------------------------------
### SQL vs NOSQL

**In the last several years, NoSQL database is getting widely adopted to solve various business problems.**

##### High-Level Differences:

* *SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.*

* *SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to..*

* *SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.*

* *SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.*

* *SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.*

* *SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb.*
------------------------------------------------------

## General Notes on NoSQL Data Modeling

* NoSQL data modeling often starts from the application-specific queries as opposed to relational modeling:
1. Relational modeling is typically driven by the structure of available data. The main design theme is “What answers do I have?”
2. NoSQL data modeling is typically driven by application-specific access patterns, i.e. the types of queries to be supported. The main design theme is “What questions do I have?” .
* NoSQL data modeling often requires a deeper understanding of data structures and algorithms than relational database modeling does.
* Data duplication and denormalization are first-class citizens.
* Relational databases are not very convenient for hierarchical or graph-like data modeling and processing. Graph databases are obviously a perfect solution for this area, but actually most of NoSQL solutions are surprisingly strong for such problems.







