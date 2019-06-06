# Install Trantrace

## Prerequisites

### Hardware Requirements

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration required:

* CPU: Intel Core or Xeon 3GHz (or Dual Core 2GHz) or equal AMD CPU
* 
* **RAM: 4 GB (6 GB recommended)**
* **Storage: 5GB**
* **Operating System: Ubuntu 16.04**

### Software Requirements

1. Apache2
2. PHP &gt;= 7.1.3
3. PHP modules: bcmath curl igbinary imap ldap mbstring memcached msgpack mysql xml xmlrpc zip
4. Mysql 5.7

## Configure

Default Setting:

| Service | port | user/password |
| :--- | :--- | :--- |
| mysql | 3306 | root/123456 |
| apache2 | 8000 | root/123456 |

* detail see [Configuration](configuration.md).

## Install Trantrace

**It is recommended to use docker-compose to install Trantrace**, which is isolated from dependency and configuration problems and easy to deploy to other servers.

### Method 1 \(Recommend\): docker-compose

* docker: [Official Guide](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

```
# for ubuntu
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $$(lsb_release -cs) stable" 
sudo apt-get update 
sudo apt-get install docker-ce docker-ce-cli containerd.io 
sudo groupadd docker && sudo usermod -aG docker $$(who am i| awk '{print \$1}')
```

* docker-compose [Official Guide](https://docs.docker.com/compose/install/)

```
# for Linux
curl -L https://github.com/docker/compose/releases/download/1.24/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

* Trantrace

  ```
  docker-compose build
  docker-compost up -d
  ```

If "OSError: cannot read the file in context: data/ca-key.pem" occurs, just delete the data directory: "**sudo rm -rf data/**"

* log: `docker-compose logs`
* stop: `docker-compose stop`
* restart: `docker-compose up -d`
* reinstall: `docker-compose up --force-recreate -d --build`
* uninstall: `docker rmi -f trantrace_web mysql:5.7 php:7.2-apache`  

### Method 2: Make

Setup myql before installation and grant root all privileges on databases.

Operating System: Ubuntu 16.04

```
make install
```

* uninstall: `make uninstall`



