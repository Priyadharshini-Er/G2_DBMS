# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS
## DATE:4/8/2023
## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```
CREATE TABLE students(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```

### OUTPUT:

![Screenshot 2023-10-03 222006](https://github.com/Priyadharshini-Er/G2_DBMS/assets/119558093/94b9b412-7662-4d5f-9b5a-35dc0cdcb33d)

### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```
ALTER TABLE students ADD Department char(10);
```

### OUTPUT:

![Screenshot 2023-10-03 222026](https://github.com/Priyadharshini-Er/G2_DBMS/assets/119558093/e1602b3d-6792-46f7-b087-ea5bfb68e21b)

### 3) Drop the student table
 
### SQL QUERY: 
```
DROP TABLE students;
```
### OUTPUT:

![Screenshot 2023-10-03 222039](https://github.com/Priyadharshini-Er/G2_DBMS/assets/119558093/41336be2-43f2-4b0a-8ca2-66c4e9691c38)

### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE students;
```

### OUTPUT:

![Screenshot 2023-10-03 222058](https://github.com/Priyadharshini-Er/G2_DBMS/assets/119558093/a9c38022-ebbd-4f43-8b0d-0ae2bba70059)

### SQL QUERY:
```
ALTER TABLE students RENAME TO mystudents;
```
### OUTPUT:
![Screenshot 2023-10-03 222112](https://github.com/Priyadharshini-Er/G2_DBMS/assets/119558093/a1089165-ee98-4a70-8bed-e916806fde88)
## RESULT:
Thus a student database has been created and DDL queries are executed successfully.
