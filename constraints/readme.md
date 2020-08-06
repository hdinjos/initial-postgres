# Constrains
## what is this?
constraints is value restrictions on table columns in sql-based databases

## 1. NOT NULL
make value column table not allowed null

example:

```sql
CREATE TABLE peoples (name text, age int not null);
```



## 2. UNIQUE
actually a constrain in which does not allow duplicate values in your particular table

example: 
in the restaurant there is a list of food menus and prices. what if the food menu is not 
double, that's the use of unique constraints

```sql
CREATE TABLE foods(name text unique, price int);
```



## 3. PRIMARY KEY
one of the constrain and it's actually important

example: 

```sql
CREATE TABLE peoples(id int primary key, name text, age int);
```



## 4. SERIAL
make automatic additions to values in the column table
usually, it use together with primary key constrain

example:

```sql
CREATE TABLE books(id serial primary key, name text, publisher text);
```



## 5. DEFAULT

example:
for fill a origin value or default value in record/row which that column is set

```sql
CREATE TABLE cars(id int, mileage int default 0);
```

this example if you insert a data in cars table, try to empty value of milage column, that fill is id only.
You can look, that milage column can't empty, but fill with zero number

this example if you insert a data in cars table, try to empty value of milage column, that fill is id only.
You can look, that milage column can't empty, but fill with zero number

## 6. FOREIGN KEY
make relation beetween tables
condition:

in store/market, a customer buy something, so store get order from customer,
in that stuation we know on order have a customer. 

conclusion we can represention
that condition into database relation, so customer will include into order table.
then  make a database: store or etc

make customers table : 

```sql
create table customers(cid int primary key, name text, contact int);
```

make order table: 

```sql
create table order(oid int primary key, item text, price int, status text, cid int references customers(cid);
```


look cid in order table become foreign key for cid in customer table