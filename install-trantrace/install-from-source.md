# Install from source

<span id='make'></span>

## Ubuntu 16.04

If {% em %}default trantrace website port (90) is occupied{% endem %}, please change 90 to other available port in conf/trantrace.apache.conf.

```sh
make install \
MYSQL_ROOT_PASSWORD=your_mysql_root_password \
MYSQL_HOST=your_mysql_host \
MYSQL_PORT=your_mysql_port
```

## Other Linux distributions and Mac

  1. Install **mysql-server (>=5.7)**, and grant root all privilege with root password.
  2. Install **apache2**.
  3. Install **PHP (>=7.1.3)** and **related PHP modules** (bcmath, curl, igbinary, imap, ldap, mbstring, memcached, msgpack, mysql, xml, xmlrpc, zip).
  4. If you want to **change trantrace website port (default: 90)**, edit port number in conf/trantrace.apache.conf.
  5. Copy source code (src/) and apache2 configure file (conf/trantrace.apache.conf) to corresponding folder.
  6. Activate website and restart apache2.
  

## Setup

open Trantrace website on Chrome, login as root with initial password 123456, and  [change password in GUI](../getting-started/registration.md#change-password).
