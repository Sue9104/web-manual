# Install

- [Requirements](#require)
  - [Operating systems](#system)
  - [Hardware](#hardware)
- [Install Trantrace](#install)
  - [Install with Docker-compose (Recommend)](#docker)
  - [Install from Source](#make)
- [Setup](#set)

## Requirements

### Operating Systems

- [install with docker-compose](#docker): Even though there are lots of operating systems supported by docker-compose, **Linux or Mac** is recommended.
- [install from source](#make): **Ubuntu 16.04** is recommended.

### Hardware

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration:

* CPU: Intel Core or Xeon 3GHz \(or Dual Core 2GHz\) or equal AMD CPU
* cores: Single \(Dual/Quad Core is recommended\)
* RAM: 4 GB \(6 GB recommended\)


## Install Trantrace
<span id='install'></span>

**It is recommended to install Trantrace with docker-compose**, which is isolated from dependency problems, and easy to deploy.

### Install with Docker-compose \(Recommend\)
<span id='docker'></span>

1. docker: [Official Guide](https://docs.docker.com/install/)
2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  
3. Configure: We stongly recommend you to change [default setting](configure.md#default) in .env, please see [Configure](configure.md).
4. install trantrace 

```
# build
docker-compose build
# start
docker-compost up -d
```

### Install from source

<span id='make'></span>

- Ubuntu 16.04
```sh
make install \
MYSQL_ROOT_PASSWORD=your_mysql_root_password \
MYSQL_HOST=your_mysql_host \
MYSQL_PORT=your_mysql_port
```

- Other Linux distribution and Mac

  1. Install **mysql-server (>=5.7)**, and grant root all privilege with root password.
  2. Install **apache2**.
  3. Install **PHP (>=7.1.3)** and **related PHP modules** (bcmath, curl, igbinary, imap, ldap, mbstring, memcached, msgpack, mysql, xml, xmlrpc, zip).
  4. If you want to **change trantrace website port (default: 90)**, change port number in conf/trantrace.apache.conf.
  5. Copy source code (src/) and apache2 configure file (conf/trantrace.apache.conf) to corresponding folder.
  6. Activate website and restart apache2.
  

## Setup

open Trantrace website on Chrome, login as root with initial password 123456, and  [change password in GUI](../getting-started/registration.md#change-password).

