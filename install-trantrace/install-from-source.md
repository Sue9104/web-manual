# Install from Source

<span id='make'></span>

Ubuntu 16.04 is recommended and installation of software dependencies is intergrated in command. However, we still provide recommend procedures for users with other Linux distributions and Mac.

## Ubuntu 16.04

```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command make install \
  MYSQL_ROOT_PASSWORD=your_mysql_root_password \
  MYSQL_HOST=your_mysql_host \
  MYSQL_PORT=your_mysql_port]
```

If default port (90) for Trantrace website is occupied, please change 90 to other available port in conf/trantrace.apache.conf.

## Other Linux distributions and Mac

  1. Install **mysql-server (>=5.7)**, grant root all privileges with root password and restart mysql service.

  ```
  **[terminal]
  **[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command mysql -u root -p  ]
  Enter password:
  Welcome to the MySQL monitor.  Commands end with ; or \g.
  Your MySQL connection id is 84975
  Server version: 5.7.24-0ubuntu0.16.04.1 (Ubuntu)
  Copyright (c) 2000, 2019, Oracle and/or its affiliates. All rights reserved.

  [warning mysql> grant all PRIVILEGES on *.* to root@'%' identified by 'your_mysql_root_password' with grant option;]
  Query OK, 0 rows affected, 1 warning (0.00 sec)

  [warning mysql> flush privileges;]
  Query OK, 0 row affected (0.00 sec)

  mysql> ^DBye
  ```
  
  2. Install **apache2**.
  
  3. Install **PHP (>=7.1.3)** and **related PHP modules** (bcmath, curl, igbinary, imap, ldap, mbstring, memcached, msgpack, mysql, xml, xmlrpc, zip).
  
  4. If you want to **change Trantrace port (default: 90)**, edit it in conf/trantrace.apache.conf.
  
  5. Copy source code (src/) and configuration file (conf/trantrace.apache.conf) to corresponding folder.
  
  6. Activate website and restart apache2.
  

## Setup

Open Trantrace on Chrome, login as root with initial password 123456, and [change password in GUI](../interface/root.md#change-password).
