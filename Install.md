### install mysql
```
sudo yum install https://repo.percona.com/yum/percona-release-latest.noarch.rpm
sudo percona-release setup ps80
sudo yum install percona-server-server
service mysql start
# cat /var/log/mysqld.log | grep generated
mysql -u root -p
alter user 'root'@'localhost' identified by '123456.xX';
```

## install redis
```
yum install redis
service redis start
```

## check
```
service redis mysql
service redis start
```
