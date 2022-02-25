# class04 Reading 
## Topics :
* SQL VS NOSQL
* sql modeling techniques
* sequelize api 

## Review, Research, and Discussion.

 **Q1 :** Name 3 advantages to Test Driven Development .
it has many advantages such as :
* **simple to debug** : In TDD when the test fails , it tells you exactly where the error is.
* **It covers the whole code parts (segments)** : each code you write it's written based on the test itself so each part of the code has at least one test.
* clearifies what the code should do before even writing the code.

**Q2 :**  In what case would you need to use beforeEach( ) or afterEach( ) in a test suite?

* beforeEach( ) used whenever you need to make a specific changes before starting each test.
* on the other hand   afterEach( ) used whenever you need to make a specific changes After each test Ends.

**Q3 :** What is one downside of Test Driven Development.

TDD can be slightly challenging and intimidating to learn, especially on your own. Understanding it completely requires a lot of dedication, practice, persistence.

**Q4:** What’s the primary difference between ES6 Classes and Constructor/Prototype Classes.

  as we know The Technical name of Javascript is Ecma Script so as we all know we use the constructors for data moduling (data representation) and the constructor is for the fifth version (ES5)  and the ES6 is an updated version of constructors but it called classes.

  also another  difference is in classes we could have a parent class and we can have a child class related (depens) on the parent class.

  **Q5:** Why REST?

  REST is representational status transfer which is to limit the client that each request the client send it suppose to follow the rule of (get - read),(post - add data), (put - update), (delete - delete).


  # Reading Summary :
  in database we have SQL and NoSQL databases each one of them has its own way to work.
  SQL stands for " structured query language " so it's a structural language that allows access to the data base while this (SQL) stores the data as Tables each table must have a schema (specific shape of representing data)
  where each row in the table should follow the schema.

  Also, the SQOL is (REDBMS) : relational database mangment system , which means The tables inside this data base are related to each other.
  Also, The SQL scaling is vertical not horizantal because the in SQL data can not be split across multiple servers.

  For the NoSQL it's unstructured query language so the data in these database are not represented as tables the representing is as documents and instead of the schema it has collections,these colloctions are json data has a key and value.
  in noSQL the data is flexable which is has not to follow a specific shape of row content data .

 The noSQL scaling is Horizantal.

 The read and write queries per second are limited for the SQl and unlimited for the noSQL.

 SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb

  Also, if the data frequently changing the SQL will be the sollution because in noSQL there are no relation between collections so you  need to change every changed data manually in the collections.
  Also, when the app are not updating the data or not too much updating at the data in the database the noSQL is the solution.


### **In conclusion** :
in general each one of them has advantages and disadvantages and there is nothing specifies which type you should go through , you can use them both it depens on the application you are creating and depens on how you want to send the data to the database.


#
### SQL modeling techniques
the SQL modeling depends on what is the relation between tables 
one to one relation.
one to many relation.
many to one relation.
many to many relation.

for this modeling the method is normalizaion for the database.

### **sequelize API** 

Sequelize is a promise-based Node.js ORM tool for Postgres, MySQL, MariaDB, SQLite, Microsoft SQL Server, Amazon Redshift, Snowflake’s Data Cloud, DB2, and IBM i.

 It features solid transaction support, relations, eager and lazy loading, read replication and more.



# preview 
* Which 3 things had you heard about previously and now have better clarity on?

    sql , nosql databases and 
modeling techniques of sql database.


* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

   sequelize API and the previuos topics.

* What are you most excited about trying to implement or see how it works?

   sequelize API.