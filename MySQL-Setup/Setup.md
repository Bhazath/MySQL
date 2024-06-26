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
