# Mysql Setup

Configration of Mysql **mysqld.cnf** to edit
```
/etc/mysql/mysql.conf.d/mysqld.conf
```

User setup 
```
create user 'gost'@'%' identified by 'RooT@123$%^'; # gost is the user

grant all on *.* to 'gost'@'%';  # granting access
```
