# Connect to mysql (mariadb) inside the container

mysql -h db -u root -pmariadb

# Create database

GRANT ALL PRIVILEGES ON *.* TO 'mariadb'@'%' IDENTIFIED BY 'mariadb' WITH GRANT OPTION;
FLUSH PRIVILEGES;

CREATE DATABASE job_lister;

SHOW DATABASES;
