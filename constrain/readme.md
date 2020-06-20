# contrain
## what is this?
constrain is value restrictions on table columns in sql-based databases

## 1. NOT NULL
make value column table not allowed null

example:
``` create table peoples (name text, age int not null);```

## 2. UNIQUE
actually a constrain in which does not allow duplicate values in your particular table

example: 
in the restaurant there is a list of food menus and prices. what if the food menu is not 
double, that's the use of unique constraints

``` create table food(name text unique, price int);```

## 3. PRIMARY KEY
one of the constrain and it's actually important
example: 

``` create table peoples(id int primary key, name text, age int);```

## 4. SERIAL
make automatic additions to values in the column table
usually,it use together with primary key constrain
example:

```create table books(id serial primary key, name text, publisher text);```
