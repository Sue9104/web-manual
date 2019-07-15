# FAQs

> Please contact [sgidrylab@protonmail.com](mailto:sgidrylab@protonmail.com) if you have more questions.

## Install

### Permisson Denied: "trantrace/data/ca-key.pem"

```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose build]
Building web
Traceback (most recent call last):
  File "site-packages/docker/utils/build.py", line 96, in create_archive
**[error PermissionError: [Errno 13] Permission denied: 'trantrace/data/ca-key.pem']

**[error OSError: Can not read file in context: trantrace/data/ca-key.pem]
[3037] Failed to execute script docker-compose
```

Cause:
  - There is a data folder under the command execution directory, and you don't have permission to read it.
  - The data folder was automatically generated when you had started this service.

Solution:
  - If you want to keep previous records, skip this step and run "docker-compose up -d".
  - Delete the data folder, and rerun it.

### Bind: address already in use

- 3307 is aleady in use
```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose up -d]
**[error listen tcp 0.0.0.0:3307: bind: address already in use]
```
    - Solution:
        - Change 3307 (DB_PORT) to other available port in .env file

- 90 is aleady in use
```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose up -d]
**[error listen tcp 0.0.0.0:90: bind: address already in use]
```
    - Solution:
        - Change 90 (WEB_PORT) to other available port in .env file

### Couldn't connect to Docker daemon

```
**[terminal]
**[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command docker-compose up -d]
**[error ERROR: Couldn't connect to Docker daemon at http+docker://localhost - is it running?]
```

Solution:
  - Check docker status: if you haven't start docker, run ```sudo service docker start```
  - Permission: if you are not in the docker group, run ```sudo usermod -aG docker $(who am i| awk '{print $1}') ```

## Forgot Password

- If you are a regular user,

    please contact administer to reset your password to 123456.

- If you are root,

    Encrypt your new password with bcrypt, and update the encrypted password to mysql table.

    **Example:**

    You are root and want to change it to "root_123456".

    ```
    **[terminal]
    **[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command htpasswd -bnBC 10 root root_123456 | cut -d: -f2 ]
    $2y$10$qvhB5CgNssUFkHIAE5bn0.1.MIVZ5SFEawRbPd/MMit9RHOFk.lFy

    **[prompt sgidrylab@ubuntu]**[path ~]**[delimiter  $ ]**[command mysql -P 3307 -u root -p  ]
    Enter password:
    Welcome to the MySQL monitor.  Commands end with ; or \g.
    Your MySQL connection id is 84975
    Server version: 5.7.24-0ubuntu0.16.04.1 (Ubuntu)
    Copyright (c) 2000, 2019, Oracle and/or its affiliates. All rights reserved.
    **[prompt mysql>]**[command use translate_01;]
    Database changed

    **[prompt mysql>]**[command update users set password = '$2y$10$qvhB5CgNssUFkHIAE5bn0.1.MIVZ5SFEawRbPd/MMit9RHOFk.lFy' where name = 'root';]
    Query OK, 1 row affected (0.00 sec)
    Rows matched: 1  Changed: 1  Warnings: 0

    **[prompt mysql>]**[command quit]
    Bye
    ```
