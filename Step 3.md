# Step 3

## Listing tables in a database

Assuming the database 'mydb' is already created, the following command will list all tables in the database 'mydb' in the MySQL server.
    
    SHOW TABLES;

### Output


| Tables in mydb |
|---------------------|
| mytable                 |

## Showing the structure of a table

Assuming the table 'mytable' in the database 'mydb' in the MySQL server is already created, the following command will show the structure of the table 'mytable' in the database 'mydb' in the MySQL server.
    
    DESCRIBE mytable;

### Output

| Field   | Type        | Null | Key | Default | Extra |
|---------|-------------|------|-----|---------|-------|
| id      | int     | NO   | PRI | NULL    | auto_increment      |
| name    | varchar(50) | YES  |     | NULL    |       |

## Condition in database queries
The where clause in the following query will filter the rows that have a name that is exactly the same as the name in the table 'mytable' in the database 'mydb' in the MySQL server.

    SELECT * FROM mytable WHERE name = 'Jane';

### Output

|id|name|
|---|---|
|1 |Jane|

### Using OR with WHERE
The following query will filter the rows that have a name that is exactly the same as the name in the table 'mytable' in the database 'mydb' in the MySQL server.

    SELECT * FROM mytable WHERE name = 'Jane' OR name = 'John';
#### Output

|id |name|
|---|---|
|1 |Jane|
|2 |John|
