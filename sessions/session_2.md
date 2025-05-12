# Session 2

CRUD Operations: a way to interact with records in a table

CRUD: 
Create - insert statement
Read - select statements
Update - update statements
Delete - delete statements

Scenario: You started a company and need to recruit employees near your location:

    CREATE DATABASE company;
    USE company;

creating a table for all employees

    CREATE TABLE employee (
        firstname VARCHAR(20),
        middlename VARCHAR(20),
        lastname VARCHAR(20),
        age INT,
        salary INT,
        location VARCHAR(20)
    );

inserting records into table

    INSERT INTO employee(firstname, middlename, lastname, age, salary, location) VALUES('Thomas', 'Alfred', 'Smith', 39, 10000, 'Zuerich');
    INSERT INTO employee(firstname, lastname, age, salary, location) VALUES('Ben', 'Miller', 24, 12500, 'Zuerich');


Value of NULL:
    Null cannot be treated as zero or as nothing,
    null means that the value is unknown


You can insert multiple records in a simple line
Example using scenario above:

    INSERT INTO employee(firstname, lastname, age, salary, location) VALUES('Albert', 'Einstein', 30, 15000, 'Zuerich'),
    ('Regula', 'Andermatt', 50, 12000, 'Bischofszell');


To prevent NULL values from being entered where they are not supposed to be there,
you can define values in a table as non-nullable in the table definition.
Leaving one of the non-nullable values empty during insertion will now return an error
Example using scenario above:

    CREATE TABLE employee (
        firstname VARCHAR(20) NOT NULL,
        middlename VARCHAR(20),
        lastname VARCHAR(20) NOT NULL,
        age INT NOT NULL,
        salary INT NOT NULL,
        location VARCHAR(20) NOT NULL
    );

Default values:
If a majority of the employees come from one location,you can add a default value to the location column;
Leaving the location column empty during insertion will result in the default value being displayed
Example using scenario above:

    CREATE TABLE employee (
        firstname VARCHAR(20) NOT NULL,
        middlename VARCHAR(20),
        lastname VARCHAR(20) NOT NULL,
        age INT NOT NULL,
        salary INT NOT NULL,
        location VARCHAR(20) DEFAULT 'Zuerich'
    );
    
SQL commands:
    
    INSERT INTO tablename VALUES();
        inserts values described in VALUES() into a table named tablename

    SELECT * FROM tablename;
        selects all data in a table named tablename

    