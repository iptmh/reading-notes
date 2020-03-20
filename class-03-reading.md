### *Class 03*

#### Why would a developer choose to make data models?
Data modeling is a more planned and structured approach than simply creating let, const or var variables on the fly. When in the world of data modeling, we want to closely watch and regulate every action that may create or change the data. 

#### What purpose do CRUD operations serve?
Create - add a new data entry
Read - recieve the contents of an existing data entry
Update - change an existing data entry
Delete - remove an existing data entry

These special functions place the standard actions of creating and reading onto rails so that they have to follow the defined structure of the data model.

#### What kind of database is Postgres? What kind of database is MongoDB?
Postgres is a SQL database. A SQL database can be thought of as more ridgid. Everything belongs in defined tables, and you use SQL to filter through those tables.
MongoDB is a NoSQL database. A NoSQL database does not impose a structure; instead it uses a system of ids to find the data you’re looking for. NoSQL databases are handy because they are much more flexible than SQL databases. 

#### What is Mongoose and why do we need it?
The package Mongoose is used as our middleman between our application and our database. Think of Mongoose as a JavaScript translator; our application speaks to Mongoose in JavaScript, and Mongoose translates that into the terms MongoDB understands. Mongoose also adds a lightweight structure and validity checking to our MongoDB, so that we get some of the benefits of an SQL database while actually using a NoSQL database.

#### Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the contraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
Each employee belongs to a team and each team belongs to a department.
