# MYSQL

### MySQL is a relational database management system (RDBMS) that uses structured query language (SQL) to manage and manipulate data

- To connet to mysql sever 
```
> mysql -u root -p # u: user and p: password 
```
- to see the databases
```
> show databases;
```
- to use the database
```
> create database <name>;
```
- To crating the table
```
CREATE TABELE <name>(
<collume> int,
<collum> varchar(255),
);
```
- Example
```
>CREATE TABLE EMPLOYEE( 
>EMPID INT,
>First Name varchar(255),
>Last Name varchar(255),
>EmpAGE int,
>EmpZone varchar(255),
);
```

-  See the strucher of the table use descripe
```
Desc <table>;
```

- How to insert data to table.
```
> INSERT INTO EMPLOYEE (First Name, Last....)
- values('jack','stone',25,'south');
```

- AUTO Increment
```
First :- > CREATE DATABASES Employee
use employee
empid int not null AUTO_INCREMENT,
FirstName varchar(255),
LastName varchar(255),
EmpAGE int,
EmpZone varcher(255),
PRIMARY KEY(empID),
);

insert into employee(firstname, last anme...)
values('jack','stone', 25, 'south');

```

