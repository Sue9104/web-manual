# FAQs

> Please contact [sgidrylab@protonmail.com](mailto:sgidrylab@protonmail.com) if you have more questions.

## install

| description | solution |
| :--- | :--- |
| OSError: can not read file in context: data/ca-key.pem | It happens when running with "docker-compose up -d --force-recreate". <br>If you want to keep prior operateion record, just delete the arguments "--force-recreate".<br> Otherwise delete the data directroy |
| listen tcp 0.0.0.0:3307: bind: address already in use | Change "DB\_PORT" in .env |
| listen tcp 0.0.0.0:8000: bind: address already in use | Change "WEB\_PORT" in .env |

## permission

| Description | Solution |
| :--- | :--- |
| user forget password | ask administer to reset password \(default: 123456\) |
| root forget password | a\) SHELL: execute _**htpasswd -bnBC 10 root new\_password\| cut -f2 -d:**_ to get encrypted\_password;<br>  b\) SQL Operation: **update users set password='encrypted\_password' where name='root'** |



