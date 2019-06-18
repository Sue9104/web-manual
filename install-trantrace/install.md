# Install

## Prerequisites

### Hardware

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration:

* CPU: Intel Core or Xeon 3GHz \(or Dual Core 2GHz\) or equal AMD CPU
* cores: Single \(Dual/Quad Core is recommended\)
* RAM: 4 GB \(6 GB recommended\)

### Operating System

- Ubuntu 16.04 for [Make](#make)
- Other System please use [docker-compose](#compose)


### Software

1. Apache2
2. PHP &gt;= 7.1.3
3. PHP modules: bcmath curl igbinary imap ldap mbstring memcached msgpack mysql xml xmlrpc zip
4. Mysql 5.7

### Browser

* Chrome

## Configure

Default Setting:

| Service | port | user/password |
| :--- | :--- | :--- |
| mysql | 3306 | root/123456 |
| apache2 | 8000 | root/123456 |

* detail see [Configure](configure.md).

## Install Trantrace

**It is recommended to use docker-compose to install Trantrace**, which is isolated from dependency problems, and easy to deploy.

### Method 1 \(Recommend\): docker-compose

<span id='compose'></span>




* docker:

  Official Guide: [https://docs.docker.com/install/linux/docker-ce/ubuntu/](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

```
# for ubuntu
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $$(lsb_release -cs) stable" 
sudo apt-get update 
sudo apt-get install docker-ce docker-ce-cli containerd.io 
sudo groupadd docker && sudo usermod -aG docker $(who am i| awk '{print $1}')
```

* docker-compose 

Official Guide: [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/)

```
# for Linux
sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

* Trantrace

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



