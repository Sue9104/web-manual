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

## Setup

open Trantrace website on Chrome, login as root with initial password 123456, and  [change password in GUI](../getting-started/registration.md#change-password).



