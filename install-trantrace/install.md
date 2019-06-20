# Install

- [Requirements](#require)
  - [Operating systems](#system)
  - [Hardware](#hardware)
- [Install Trantrace](#install)
  - [Install with Docker-compose (Recommend)](#docker)
  - [Install from Source](#make)

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

If you are using Ubuntu 16.04, we strongly recommend to install using 
```make install MYSQL_ROOT_PASSWORD=your_mysql_root_password MYSQL_HOST=your_mysql_host MYSQL_PORT=your_mysql_port```.
 
Otherwise, you should manually install **mysql, apache2, php and related modules** first, then copy source code folder ('src/') to corresponding folder, lastly activate the webiste and restart apache2.

Software Dependencies:
1. Mysql: install mysql-server(mysql>=5.7) and start mysql service, then grant root all privileges.
2. Apace2
3. PHP >= 7.1.3
4. PHP-modules: bcmath, curl, igbinary, imap, ldap, mbstring, memcached, msgpack, mysql, xml, xmlrpc, zip


