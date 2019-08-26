# Install from Source Code

<span id='make'></span>

**Ubuntu 16.04 is recommended and the installation of dependencies and Trantrace are integrated in makefile.** However, we still provide recommend procedures for users with other Linux distributions and Mac.

## Ubuntu 16.04

```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command make install \
  MYSQL_ROOT_PASSWORD=your_mysql_root_password \
  MYSQL_HOST=your_mysql_host \
  MYSQL_PORT=your_mysql_port]
```

Please change 90 to other available port in conf/trantrace.apache.conf if it is occupied.

## Other Linux distributions and Mac

  1. Install **mysql-server (>=5.7)**, and grant root (MySQL administrator) all privileges with root password. Then restart MySQL.

  ```
  **[terminal]
  **[prompt sgidrylab@centos]**[path ~]**[delimiter  $ ]**[command mysql -u root -p  ]
  Enter password:
  Welcome to the MySQL monitor.  Commands end with ; or \g.
  Your MySQL connection id is 84975
  Copyright (c) 2000, 2019, Oracle and/or its affiliates. All rights reserved.

  **[prompt mysql>]**[command grant all PRIVILEGES on *.* to root@'%' identified by 'your_mysql_root_password' with grant option;]
  Query OK, 0 rows affected, 1 warning (0.00 sec)

  **[prompt mysql>]**[command flush privileges;]
  Query OK, 0 row affected (0.00 sec)

  **[prompt mysql>]**[command quit]
  Bye
  **[prompt sgidrylab@centos]**[path ~]**[delimiter  $ ]**[command sudo service mysql restart]
  ```
  
  2. Install **apache2**.
  
  3. Install **PHP (>=7.1.3)** and **related PHP modules** (bcmath, curl, igbinary, imap, ldap, mbstring, memcached, msgpack, mysql, xml, xmlrpc, zip).
  
  4. If you want to **change Trantrace port (default: 90)**, edit it in conf/trantrace.apache.conf.
  
  5. Copy source code (src/) and configuration file (conf/trantrace.apache.conf) to corresponding folder.
  
  6. Activate the website and restart apache2.
  

## Setup

> #### Warning:: Security Warning
>
> Please change the administrator password in GUI immediately.

The built-in administrator account email and password are root and 123456 respectively. Log in Trantrace as an administrator and [change password in GUI](../interface/root.md#change-password).

