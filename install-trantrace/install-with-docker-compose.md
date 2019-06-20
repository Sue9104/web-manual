# Install Trantrace with Docker-compose

<!-- toc -->

**It is recommended to install Trantrace with docker-compose**, which is isolated from dependency problems, and easy to deploy.

## Prerequisites

1. docker: [Official Guide](https://docs.docker.com/install/)

2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  


## Configure

We stongly recommend you to change default root password in ".env" file for security.

| Service | Setting | Default | How to change |
| :--- | :--- | :--- | :--- |
| Mysql | root password | 123456 | edit "DB\_PASSWORD" in .env |
| Mysql | port | 3307 | edit "DB\_PORT" in .env |
| Trantrace | port | 90 | edit "WEB\_PORT" in .env |

## Install

```sh 
# install
docker-compose build
# start
docker-compost up -d
```

Please see [docker-compose offical guide](https://docs.docker.com/compose/reference/overview/) for more operations.

## Setup

open Trantrace website on Chrome, login as root with initial password 123456, and  [change password in GUI](../getting-started/registration.md#change-password).
