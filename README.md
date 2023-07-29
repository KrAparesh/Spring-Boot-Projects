# What do we hope to gain?

Using a database to save our coffee details.


# Understanding terms 

## Java Persistence API

Java Persistence API (_JPA_) is a specification that lets you do Object-Relational Mapping. What ORM does is let you map your entity classes into sequel tables so that when you connect to the database, you provide some kind of metadata on your entity classes so you don't have to do the query and mapping for you. JPA is the spec that lets you configure your entity classes and give it to a framework that does the rest. It makes working with relational database easier.

## @Entity

We need to create a table in the **relational database** and we want the table name to be the class name. This is where we use the _@Entity_ tag (Placing it right above the class).

This will create a table name same as the class name with the member variables as it's column, and each instance of the class (objects) shall be it's rows.

## @Id

Each table must have a primary key. We use the *@Id* annotation to mark the datatype below it as the Key datatype. 

More to be added...

