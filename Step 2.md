# How to Create Tables in a Database

## Creating a Table
-------------------
The following command will create a table called 'mytable' in the database 'mydb' in the MySQL server.

    CREATE TABLE mytable (
         id INT NOT NULL AUTO_INCREMENT,
         name VARCHAR(50) NOT NULL,
         PRIMARY KEY (id)
    );

## Accessing a Table
-------------------
The following command will use the table 'mytable' in the database 'mydb' in the MySQL server.

    SELECT * FROM mytable;

### Output

| id    | name |
|----   |------|
| null  | null |

## Inserting Data into a Table
-------------------------------
The following command will insert data into the table 'mytable' in the database 'mydb' in the MySQL server.

    Example:
    
    INSERT INTO mytable (name) VALUES ('John');
    INSERT INTO mytable (name) VALUES ('Jane');
    INSERT INTO mytable (name) VALUES ('Jack');
    INSERT INTO mytable (name) VALUES ('Jill');
    INSERT INTO mytable (name) VALUES ('Jenny');
    

### Output
    Now the table after SELECT * FROM mytable is:
    
| id | name    |
|----|---------|
|  1 | John    |
|  2 | Jane    |
|  3 | Jack    |
|  4 | Jill    |
|  5 | Jenny   |

[< PREVIOUS](https://github.com/bijomathewjose/MySQL-Starter-Pack/blob/development/Step%201.md)
[AFTER >](https://github.com/bijomathewjose/MySQL-Starter-Pack/blob/development/Step%203.md)




