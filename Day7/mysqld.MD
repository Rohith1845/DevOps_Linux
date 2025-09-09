Developer has choosen the MySQL database. Hence, we are installing it

Database
========
Database server -> it is physical server
server == Box == Node

Databse server should be installed

- dnf install mysql-server -y

start mysql server
- systemctl enable mysqld
- systemctl status mysqld

we need to change the default root password in order to start using mysql-server

mysql_secure_installation

Verification :

We can check data by using cilent package called mysql 
command to connect with server

mysql -h <host-address> -u root -p<password>
if you are working in same server no need of host-address

But if you and cilent are in same server you can simply use
-mysql

-show databases -> to get visibility of schemas/ databases

-show tables -> to see list of tables

you can get entires of tables:
select * from schema/database