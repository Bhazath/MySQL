# Mysql Setup

- Configration of Mysql **mysqld.cnf** to edit
```
/etc/mysql/mysql.conf.d/mysqld.conf
```

- edit the bind address
```
# localhost which is more compatible and is not less secure.
bind-address            = 0.0.0.0  # To ZERO
mysqlx-bind-address     = 127.0.0.1
```

- User setup 
```
create user 'gost'@'%' identified by 'RooT@123$%^'; # gost is the user

grant all on *.* to 'gost'@'%';  # granting access
```
# 
# 

## To see all Show user in mysql
1) Log in to MySQL: Open your terminal or command prompt and log in to the MySQL server.

```
mysql -u root -p
```
You will be prompted to enter the password for the MySQL root user (or the user you specified).

2) Select the mysql database: Switch to the mysql database where the user information is stored.
```
USE mysql;
```
3) Query the user table: Run the following SQL query to see a list of all users.

```
SELECT User, Host FROM user;
```
