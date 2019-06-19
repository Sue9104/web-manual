# Install

- [Requirements](#require)
  - [Operating Systems](#system)
  - [Hardware](#hardware)
- [Install Trantrace](#install)
  - [Configure](#config)
  - [Install using docker-compose](#docker)
  - [Install using make](#make)



## Requirements

### Operating Systems


- Ubuntu 16.04 using [Make](#make)
- Other System please use [docker-compose](#docker)

### Hardware

Actual requirements vary heavily based on translation database size and user amount, the following is the minimal configuration:

* CPU: Intel Core or Xeon 3GHz \(or Dual Core 2GHz\) or equal AMD CPU
* cores: Single \(Dual/Quad Core is recommended\)
* RAM: 4 GB \(6 GB recommended\)



## Install Trantrace
<span id='install'></span>

**It is recommended to use docker-compose to install Trantrace**, which is isolated from dependency problems, and easy to deploy.

## Configure
<span id='config'></span>

Default Setting:

| Service | port | user/password |
| :--- | :--- | :--- |
| mysql | 3306 | root/123456 |
| apache2 | 8000 | root/123456 |

* If you want revise this setting, please see [Configure](configure.md).


### Method 1 \(Recommend\): docker-compose
<span id='docker'></span>

1. docker is required for docker-compose: [Official Guide](https://docs.docker.com/install/)
2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  
3. install and start trantrace 

```
# build
docker-compose build
# start
docker-compost up -d
```

### Method 2: Make

<span id='make'></span>

1. Mysql: Setup and grant root all privileges on databases.
2. Apache2: ```make apache2```
3. PHP and PHP modules: ```make php php-modules```
4. Install Trantrace: ```make install```


