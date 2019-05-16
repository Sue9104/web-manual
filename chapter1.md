# Getting Started

## Requirements

### Hardware Requirements

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration required:

* **CPU: 2 cores**
* **Memory: 2 GB RAM**
* **Storage: 5GB**
* **Operating System: Ubuntu 16.04**

### Software Requirements

1. Apache2

```
sudo apt update 
sudo apt install apache2
sudo a2enmod rewrite
sudo a2enmod headers
```

2. PHP >= 7.1.3

```
sudo add-apt-repository ppa:ondrej/php
sudo apt update
sudo apt install php7.2
```

 - PHP modules
 
```
sudo apt install php7.2-fpm php7.2-mysql php7.2-curl php7.2-gd php7.2-mbstring php7.2-xml php7.2-xmlrpc php7.2-zip php7.2-opcache -y
```

3. Mysql

```
sudo apt-get install mysql-server
sudo apt isntall mysql-client
sudo apt install libmysqlclient-dev
```

4. Other system requirements

## Installation

### Installing with comand line tools

```sh
make install
```

### Installing with docker

```
docker-compose up
```



