# Install

## Requirements

### Operating Systems

- Ubuntu 16.04 for [Make](#make)
- Other System please use [docker-compose](#compose)

### Browser

* **Chrome:** https://chromereleases.googleblog.com/


### Hardware

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration:

* CPU: Intel Core or Xeon 3GHz \(or Dual Core 2GHz\) or equal AMD CPU
* cores: Single \(Dual/Quad Core is recommended\)
* RAM: 4 GB \(6 GB recommended\)



## Install Trantrace

**It is recommended to use docker-compose to install Trantrace**, which is isolated from dependency problems, and easy to deploy.

## Configure

Default Setting:

| Service | port | user/password |
| :--- | :--- | :--- |
| mysql | 3306 | root/123456 |
| apache2 | 8000 | root/123456 |

* If you want revise this setting, please see [Configure](configure.md).


### Method 1 \(Recommend\): docker-compose

<span id='compose'></span>

1. docker is required for docker-compose: [Official Guide](https://docs.docker.com/install/)
2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  
3. install trantrace using trantrace

```
# build
docker-compose build
# start
docker-compost up -d
```

### Method 2: Make

<span id='make'></span>


* Mysql

Setup myql before installation and grant root all privileges on databases.


* Trantrace

make command is specific for Ubuntu 16.04, other systems may have some depencies problems.

```
make install
```



### Software

1. Apache2
2. PHP &gt;= 7.1.3
3. PHP modules: bcmath curl igbinary imap ldap mbstring memcached msgpack mysql xml xmlrpc zip
4. Mysql 5.7

