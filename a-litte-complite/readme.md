## make a database
```
CREATE DATABASE a_database;
```
example: CREATE DATABASE school;

## list all database
```
\l
```
## enter to database
```
\c a_database
```
## create table
```
CREATE TABLE a_table(data1 data_type,data2 data_type,data3 data_type,etc);
```

example: CREATE TABLE students(id int, name text, age int, address text);
## list all table on a database
```
\dt
```
## insert value to table
```
INSERT INTO a_table(data1,data2,data3,etc) VALUES (value1,value2,value3,etc);
```
example: INSERT INTO students(id,name,age,address) VALUES (5,'Yuda Saputra',23,'Pati'); 
## list all data on table
```
SELECT * FROM a_table;
```
example: SELECT * FROM students;
