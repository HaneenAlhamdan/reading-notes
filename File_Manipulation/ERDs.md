 ## ERDs

### What is an Entity Relationship Diagram?

Entity relationship diagrams are customized flowcharts that illustrate the ways in which 'entities' ' people,companies, concepts, information, objects ' relate to each other within a set system.
They use a defined set of simple symbols, such as rectangles, diamonds, circles and squares, linked by a variety of lines to represent the interconnectedness of entities, their attributes and their various relationships. Although simple diagrams have been used by many cultures for millennia, the development of ERDs as they apply to business and data management began in the 1960s and 1970s with the work of Peter Chen, Charles Bachman and A.P.G. Brown.

* DataType: attribute is used to specify a data type that's more specific than the database intrinsic type.

* StringLength: Attribute Specifies both the Min and Max length of characters that we can use in a field. StringLength is somewhat similar to MaxLength and MinLength attribute but operates only on string type properties..

* Column attribute: can be applied to one or more properties in an entity class to configure the corresponding column name, data type and order in a database table.

* Required attribute makes the name properties required fields.
* The CourseAssignments and OfficeAssignment properties are navigation properties.

* DatabaseGenerated : The DatabaseGenerated attribute specifies how values are generated for a property by the database. The attribute takes a DatabaseGeneratedOption enumeration value, which can be one of three values:

1. Computed
2. Identity
3. None

### What is DBMS?

A DBMS is a software that allows creation, definition and manipulation of database, allowing users to store, process and analyse data easily. DBMS provides us with an interface or a tool, to perform various operations like creating database, storing data in it, updating data, creating tables in the database and a lot more.
DBMS also provides protection and security to the databases. It also maintains data consistency in case of multiple users.

### A modern DBMS has the following characteristics :−

1. Query Language :– It is more efficient to retrieve and manipulate data. Traditionally it was not possible where file-processing system was used.

2. Consistency :– DBMS helps to achieve consistency as compared to earlier forms of data storing applications like file-processing systems.

3. Security :– DBMS offers many different levels of security features, which enables multiple users to have different views with different features.

4. ACID Properties :– DBMS follows the concepts transactions, i.e., ACID properties : Atomicity, Consistency, Isolation, and Durability.

### The users of a DBMS can be broadly categorized as follows :−

![download (3)](https://user-images.githubusercontent.com/98957434/162646168-3aa7f186-8b4b-4f49-9beb-084e1d460801.png)

* A Foreign Key
You can use constraints to enforce restrictions on the data in a DataTable , in order to maintain the integrity of the data. A ForeignKeyConstraint can restrict, as well as propagate, changes to related columns.

* Composite key
The key to a composite pattern is an abstract class that represents both primitives (individual objects) and their containers (compositions of objects). Define an abstract base class (Component) that specifies the behavior that needs to be exercised uniformly across all primitive and composite objects. Subclass the Primitive and Composite classes off of the Component class. Each Composite object "couples" itself only to the abstract type Component as it manages its "children". 
