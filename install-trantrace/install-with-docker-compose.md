# Install Trantrace with Docker-compose \(Recommend\)

<!-- toc -->

**It is recommended to install Trantrace with docker-compose**, which is isolated from dependency problems, and easy to deploy.

## Install docker-compose

<span id='docker'></span>

1. docker: [Official Guide](https://docs.docker.com/install/)

2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  


## Configure

We stongly recommend you to change default setting in ".env" file for security.





## Install Trantrace

```
# build
docker-compose build
# start
docker-compost up -d
```

Please see docker-compose offical Guide for more operation.

## Setup

open Trantrace website on Chrome, login as root with initial password 123456, and  [change password in GUI](../getting-started/registration.md#change-password).



# Configure

## Default Setting

|  | Service | adminstrator | administrator password |
| :--- | :--- | :--- | :--- |
| mysql | 3306 | root | 123456 |
| Trantrace | 90 | root | 123456 |

## How to Change

### Mysql

| Setting | How to change |
| :--- | :--- |
| port | revise "DB\_PORT" in .env |
| root password | revise "DB\_PASSWORD" in .env |


* Once the  website is started, you need restart after edit.
* More SQL operation, please see MySQL Official Guide: [https://dev.mysql.com/doc/refman/5.7/en/](https://dev.mysql.com/doc/refman/5.7/en/)

### Trantrace

| Setting | How to change |
| :--- | :--- |
| port | revise "WEB\_PORT" in .env |
| root password | loggin with initialize accout\(root/123456\), and [change password in GUI](../getting-started/registration.md#change-password) |



