# Session 1

relational database = 
    - data is stored in the form of rows and columns
    - tables have relations between each other
    - Examples: MySQL, SQLServer, PostgreSQL, SQLLite


non-relational (NO SQL) database = 
    - Not stored in form of rows/columns
    - each table is different and they don't have relations with each other
    - Examples: HBase, MongoDB, Cassandra


Course will be handling MySQL

SQL = Structured Query Language (used to query a relational DB)
    Used to interact with structured data (rows/columns)

MySQL = Database 
SQL = Method to interact with data in MySQL

datatypes:

int = numeric
varchar = string

SQL commands:

    SHOW DATABASES;
        shows all databases created 

    CREATE DATABASE name;
        creates a database named name

    DROP DATABASE name;
        deletes a database named name
    
    USE name;
        "moves" into a database named name, 
        all commands will be executed in name
    
    SELECT DATABASE();
        shows what database you're currently in

    CREATE TABLE tablename;
        creates a table in the current database 
        named tablename

        Example:
        CREATE TABLE employee(name VARCHAR(50), age INT, salary INT)

    SHOW TABLES;
        shows all tables in current database

    DESCRIBE tablename; || DESC tablename;
        shows structure of a table named tablename

    DROP TABLE tablename;
        deletes a table named tablename

    

    