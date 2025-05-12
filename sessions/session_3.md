# Session 3

Primary Key = used to uniquely identify each record in the table

Implementation:

    CREATE TABLE employee (
		id INT PRIMARY KEY,
        firstname VARCHAR(20) NOT NULL,
        middlename VARCHAR(20),
        lastname VARCHAR(20) NOT NULL,
        age INT NOT NULL,
        salary INT NOT NULL,
        location VARCHAR(20) NOT NULL DEFAULT 'Zuerich'
    );

by using the tag PRIMARY KEY we identify the variable as the primary key

Auto Increment Keys = 
Unique Key = 