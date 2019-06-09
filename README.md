# Kali_learning

## HTTP

### 激活Apache HTTP服务

```
root@kali:~# /etc/init.d/apache2 start
[ ok ] Starting apache2 (via systemctl): apache2.service.
```
或者

```
service sqpche2 start
```

但这样没有系统提示.

从浏览器看到结果如下:

![](https://github.com/444749308/Kali_learning/blob/master/picture/1.PNG)


### 停止Apache HTTP服务

```
root@kali:~# /etc/init.d/apache2 stop
[ ok ] Stopping apache2 (via systemctl): apache2.service.
```

或者

```
service sqpche2 stop
```

但这样没有系统提示.
### 开机自动启用 Apache HTTP 服务

```
root@kali:~# vi /etc/rc.local 
```

```
/etc/init.d/ssh start
exit 0
```

rc.local为开机加载文件

## MySQL

### 启动 MySQL服务

```
root@kali:~# service mysql start

```

### 登陆MySQL服务器

```
root@kali:~# mysql -u root -p
Enter password: 
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 49
Server version: 10.3.13-MariaDB-1 Debian buildd-unstable

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> Ctrl-C -- exit!
Aborted

```
### MySQL开机自启动


```
root@kali:~# vi /etc/rc.local 
```

插入一行

```
/etc/init.d/mysql start
```

## 
