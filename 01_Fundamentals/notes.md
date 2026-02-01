INTRODUCTION:
S-Q-L : Structured Query Language
->It is Language we use to communicate with Databases :) 
-> It can refine and transform data, trying to make sense of the raw numbers and records turning them into information that people can understand and use

Databases : a database is an organized collection of structured information, made up of tables that hold rows and columns of data
-> tables are the backbone of data organization and management
-> A database table consists of several elements that define how data is stored and accessed
-> Here are the primary components:
1. Columns(also known as fields) : -> it represents the attributes of the data stored in the table
             -> Each column has a specific data type that defines the kind of data it can hold, such as integers, strings, dates, or binary data
   Example : A "Customer" table has columns for CustomerID, FirstName, LastName, Email and DOB
2. Rows(also known as records) : -> represent individual data entries in the table
                                 -> Each row contains a unique combination of values for the columns
   Example: A row in the "Customer" table might contain the values: 1, John, Doe, john.doe@example.com and 1980-05-15
3. Primary Key(PK) (A primary key is a column or a set of columns uniquely identifying each row in the table): -> It ensures that no two rows have the same primary key value
   Example: In the "Customer" table, the CustomerID column could be the primary key
4. Data Types (Data types define the kind of data that can be stored in each column) : -> Common data types include INT, VARCHAR (NVARCHAR), DATE  (DATETIME), DECIMAL (NUMERIC) and BOOLEAN
   Example: The Email column in the "Customer" table might store variable-length string data using the VARCHAR data type
5.Constraints (Constraints are rules applied to columns to enforce data integrity and consistency): ->Common constraints include NOT NULL, UNIQUE, CHECK and FOREIGN KEY
   Example: The Email column might have a UNIQUE constraint to ensure that no two customers have the same email address.

Understanding Table Relationships: -> In a database, tables are often related to each other through keys and relationships
                                   -> These relationships help maintain data integrity and support complex queries

a) Foreign Key(A foreign key is a column or a set of columns in one table that refers to the primary key in another table): ->It establishes a link between the two tables.
   Example: In an "Invoice" table, the CustomerID column might be a foreign key referencing the CustomerID column in the "Customer" table.

b) One-to-Many Relationship(A row in one table can be associated with multiple rows in another in a one-to-many relationship)
   Example: A customer can place multiple orders, creating a one-to-many relationship between the "Customer" table and the "Invoice" table.

c) Many-to-Many Relationship(In a many-to-many relationship, multiple rows in one table can be associated with multiple rows in another) ->These relationships are typically implemented using a junction table
   Example: Students and courses in a school database can have a many-to-many relationship, where students can enroll in multiple classes and each course can have multiple students.

