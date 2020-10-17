# Read 04

## Review

1-Why would a developer choose to make data models?
    Faster performance
    Better organization

2-What purpose do CRUD operations serve?
    Create Update Read Delete data from the database

3- What kind of database is Postgres? What kind of database is MongoDB?

    Postgres is SQL
    MongoDB is NoSQL

4-What is Mongoose and why do we need it?
    Mongoose is a library for MongoDB you can get from npm.
    It basically offers the organization between data.

## Preview

- Which 3 things had you heard about previously and now have better clarity on
SQL
Schema
Mongoose

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
NoSQL
Mongoose
Data modeling

- What are you most excited about trying to implement or see how it works?
Mongoose

## Preparation summary

### Repository Design Pattern

In using the Repository design pattern, you can hide the details of how the data is eventually stored or retrieved to and from the data store. This data store can be a database, an xml file, etc. You can apply this design pattern to even hide how data that is exposed by a web service or an ORM is accessed

### In-Memory testing

In-memory database pros & cons

Pros:

No need for mocks: Your code is directly executed using the in-memory database, exactly the same as using your regular database.

Faster development: Given that I don't need to build a mock for every operation and outcome but only test the query, I found the development process to be faster and more straightforward.
More reliable tests: You're testing the actual code that will be executed on production, instead of some mock that might be incorrect, incomplete or outdated.
Tests are easier to build: I'm not an expert in unit testing and the fact that I only need to seed the database and execute the code that I need to test made the whole process a lot easier to me.
Cons:

The in-memory database probably needs seeding
More memory usage (dah)
Tests take longer to run (depending on your hardware).
