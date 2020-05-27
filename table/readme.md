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
## distinct clausa (filter the data origin in columns that same data will count one)
```
SELECT DISTINCT column_table FROM table;
```
example: SELECT DISTINCT name FROM students;
## search data based on column
```
SELECT * FROM table WHERE column_name='search_data';
```
example: (1) SELECT * FROM students WHERAE name='yuda';
        (2) SELECT * FROM students WHERE age<22; (can also use comparison operator);
if the data you are looking does not match, then postgresql will not output anything
## search data base on column *except*
```
SELECT * FROM table WHERE NOT column_name='search_data';
```
example: (1) SELECT * FROM students WHERAE NOT name='yuda';
        (2) SELECT * FROM students WHERE NOT age<22; (can also use comparison operator);
this query same above, but will produce data that is the opposite of what we are searching
