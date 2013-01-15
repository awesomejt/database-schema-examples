Database Schema Examples
========================

This project is an open-source (Apache License 2.0) collection of data models and SQL scripts for creating sample database
schemas. This project was started after a bit of searching for an existing project without much success.

**Project Benefits**
+ SQL scripts for creating schemas and sample data for testing or proof-of-concept applications
+ A way to teach developers how to write DDL/SQL
+ A database schema design starting point

**Database examples should contain the following:**
+ README file to discribe the purpose of the example, how to use the SQL scripts, and anything else required.
+ ER diagram or other database model PNG image
+ ER diagram source file (optional)
+ Schema creation SQL (DDL) scripts
+ Sample data insertion scripts (optional)
+ Schema removal scripts
+ Database system specific scripts (create database, schema, users/permissions, constraints, etc)



Getting Started
---------------

To use the existing examples, clone the entire project or use GitHub to navigate down into the appropriate
folder and copy specific scripts as needed. Each folder should have a description regarding the example's 
purpose and design.

Scripts are organized by database system (MySQL, Derby, DB2, etc) and purpose (create, data, drop). Example
authors are encouraged to create a database-independent version (ANSI/ISO SQL) if possible (generic_create.sql), but many 
times this is not practical.

Contributing
------------

We welcome contributions! All contributions must be original work and willing to be released under the 
Apache License 2.0 (liberal open source).

### Common SQL Syntax (When Possible)

Most modern database systems understand some level of ANSI or ISO SQL standard syntax. However most 
databases stray from the standard in some unforgivable way. Still, it may be possible to build a schema
in a common syntax that is understood by many systems.

Common or generic database scripts should be named with the "generic" prefix in the filename. Example:
*generic_schema_create.sql*.

### Database Specific Syntax

There are many cases when database specific syntax is required or strongly desired. The preferred approach
is to use database-specific scripts to alter an existing schema already created with generic scripts. As
a last resort, a completely database specific approach may be used. Either way, document the approach taken
with each schema example.

Name database-specific files with a reasonable prefix. Example: *mysql_schema_create_alter.sql*.

### Database Models

Creating database models (Entity-Relationship (ER) Diagrams) are useful when provided. Please use a freely available
tool for creating a saving ER diagram files. Also, always export the ER diagram as a PNG image file so others can 
view the diagram without using a specific tool.

