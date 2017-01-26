# Description

FreeRadius WebGUI Interface. It uses the MySQL database from FreeRADIUS

# Run the image

$ run -d -t daloradius -p 80:80 -e DB_HOST_VALUE=mysql.server stejon/daloradius

# Environment variables

- DB_HOST_VALUE=localhost
- DB_PORT_VALUE=3306
- DB_USER_VALUE=radius
- DB_PASS_VALUE=radpass
- DB_NAME_VALUE=radius

# Notes

MySQL server specific configuration.

```
[mysqld]
sql_mode = STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION
```
