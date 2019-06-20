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
| sql\_mode | revise "--sql-mode" in docker-compose.yaml |

* Once the  website is started, you need restart after edit.
* More SQL operation, please see MySQL Official Guide: [https://dev.mysql.com/doc/refman/5.7/en/](https://dev.mysql.com/doc/refman/5.7/en/)

### Trantrace

| Setting | How to change |
| :--- | :--- |
| port | revise "WEB\_PORT" in .env |
| root password | loggin with initialize accout\(root/123456\), and [change password in GUI](../getting-started/registration.md#change-password) |



