
## Entity Framework and APIs

### MVC

ASP.NET MVC 5 is a web framework based on Model-View-Controller (MVC) architecture. Developers can build dynamic web applications using ASP.NET MVC framework that enables a clean separation of concerns, fast development, and TDD friendly.
As per the official definition, Model-View-Controller (MVC) is a software architectural pattern for implementing user interfaces. It divides a given software application into three interconnected parts, so as to separate internal representations of information from the ways that information is presented to or accepted from the user.

### What is Entity Framework?

 It is to abstract the ties to a relational database, in such a way that the developer can relate to the database entity as to a set of objects and then to classes in addition to their properties. In essence, we speak about decoupling between our Applications and the logic of data access, which proves to be a major plus. For example: If we need to move - in the context of a single program - to different manufacturers database, it would be required to review the way and the instructions with which we interface the data manager on duty.
 
## The Entity Framework provides three approaches to create an entity model and each one has their own pros and cons.
1. Database First
2. Model First
3. Code First


## WHAT IS SEED DATA APPROACH IN ENTITY FRAMEWORK?
Sometimes, you may want to insert some dummy data into database table while initialized database. These dummy data might be for the testing purpose. Seed Data Approach lets you insert dummy records into a table. In this tutorial, you will learn Entity Framework Seed Database Approach with easy programming examples

There are some conditions when seeding data to the database. These conditions are:

1. You must check whether or not the target database already exists.

2. If target database exists then current code first model is compared to the model stored in metadata in the existing database.

3. If current model doesn’t match with the existing model then database gets dropped.

4. Then the database is recreated.