```
-- Log in to MySQL as root
mysql -u root -p

-- Create the scott database
CREATE DATABASE scott;

-- Use the scott database
USE scott;

-- Create the emp table
CREATE TABLE emp (
    empno INT(4) PRIMARY KEY,
    ename VARCHAR(10),
    job VARCHAR(9),
    mgr INT(4),
    hiredate DATE,
    sal DECIMAL(7, 2),
    comm DECIMAL(7, 2),
    deptno INT(2)
);

-- Insert data into the emp table
INSERT INTO emp (empno, ename, job, mgr, hiredate, sal, comm, deptno) VALUES
(7369, 'SMITH', 'CLERK', 7902, '1980-12-17', 800.00, NULL, 20),
(7499, 'ALLEN', 'SALESMAN', 7698, '1981-02-20', 1600.00, 300.00, 30),
(7521, 'WARD', 'SALESMAN', 7698, '1981-02-22', 1250.00, 500.00, 30),
(7566, 'JONES', 'MANAGER', 7839, '1981-04-02', 2975.00, NULL, 20),
(7654, 'MARTIN', 'SALESMAN', 7698, '1981-09-28', 1250.00, 1400.00, 30),
(7698, 'BLAKE', 'MANAGER', 7839, '1981-05-01', 2850.00, NULL, 30),
(7782, 'CLARK', 'MANAGER', 7839, '1981-06-09', 2450.00, NULL, 10),
(7788, 'SCOTT', 'ANALYST', 7566, '1987-04-19', 3000.00, NULL, 20),
(7839, 'KING', 'PRESIDENT', NULL, '1981-11-17', 5000.00, NULL, 10),
(7844, 'TURNER', 'SALESMAN', 7698, '1981-09-08', 1500.00, 0.00, 30),
(7876, 'ADAMS', 'CLERK', 7788, '1987-05-23', 1100.00, NULL, 20),
(7900, 'JAMES', 'CLERK', 7698, '1981-12-03', 950.00, NULL, 30),
(7902, 'FORD', 'ANALYST', 7566, '1981-12-03', 3000.00, NULL, 20),
(7934, 'MILLER', 'CLERK', 7782, '1982-01-23', 1300.00, NULL, 10);

```

# Dept
```
CREATE TABLE dept (
    deptno INT PRIMARY KEY,
    dname VARCHAR(14),
    loc VARCHAR(13)
);

-- Insert data into the dept table
INSERT INTO dept (deptno, dname, loc)
VALUES (10, 'ACCOUNTING', 'NEW YORK');

INSERT INTO dept (deptno, dname, loc)
VALUES (20, 'RESEARCH', 'DALLAS');

INSERT INTO dept (deptno, dname, loc)
VALUES (30, 'SALES', 'CHICAGO');

INSERT INTO dept (deptno, dname, loc)
VALUES (40, 'OPERATIONS', 'BOSTON');
```

# salgrade
```
-- Create the salgrade table
CREATE TABLE salgrade (
    grade INT PRIMARY KEY,
    losal INT,
    hisal INT
);

-- Insert data into the salgrade table
INSERT INTO salgrade (grade, losal, hisal)
VALUES (1, 700, 1200);

INSERT INTO salgrade (grade, losal, hisal)
VALUES (2, 1201, 1400);

INSERT INTO salgrade (grade, losal, hisal)
VALUES (3, 1401, 2000);

INSERT INTO salgrade (grade, losal, hisal)
VALUES (4, 2001, 3000);

INSERT INTO salgrade (grade, losal, hisal)
VALUES (5, 3001, 9999);

```

# Bonus
```
CREATE TABLE bonus (
    ename VARCHAR(10),
    job VARCHAR(9),
    sal DECIMAL(7, 2),
    comm DECIMAL(7, 2),
    deptno INT
);

```
