# Install Trantrace with Docker-compose

**It is recommended to install Trantrace with docker-compose**, which is isolated from dependency problems and easy to deploy.

## Prerequisites

Docker is required for docker-compose, please make sure both are installed.

1. docker: [Official Guide](https://docs.docker.com/install/)

2. docker-compose: [Official Guide](https://docs.docker.com/compose/install/)  


## Configure

> **[warning] Please change the default mysql root password in ".env" file for security. **

| Service | Setting | Default | How to change |
| :--- | :--- | :--- | :--- |
| Mysql | root password | 123456 | edit "DB\_PASSWORD" in .env |
| Mysql | port | 3307 | edit "DB\_PORT" in .env |
| Trantrace | port | 90 | edit "WEB\_PORT" in .env |

## Install

```
**[terminal]
# Build Trantrace
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose build]
# Start Trantrace
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose up -d]
```

For more operations, please see [docker-compose official guide](https://docs.docker.com/compose/reference/overview/).

## Setup

Login Trantrace as root with initial password 123456, and [change password in GUI](../interface/root.md#change-password).
