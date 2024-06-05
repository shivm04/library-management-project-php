## Clone this repository
```
  git clone https://github.com/shivm04/hostel-management-project-PHP.git
```

## Required Packages 
```
PHP 8 Version 
Mysql 8 Version
Install PHP required Modules
Apache2
```

## Create a databases 
```
  DB name :- hostel
  CREATE DATABASE hostel;

  Import the hostel.sql file into the hostel database
  mysql -u root -p hostel < hostel.sql

```

## Chnage the permission of the files 
```
chmod -R 755 hostel-management-project-PHP/ hostel-management-project-PHP/*
chown -R www-data:root hostel-management-project-PHP/* hostel-management-project-PHP/
```

## Change the database Credentials in the configuration file 
```
   hostel-management-project-PHP/hostel/includes
   hostel-management-project-PHP/hostel/admin/includes
```

## Create a config file for the apache to host our website 

```
<VirtualHost *:80>
    ServerAdmin webmaster@your_domain.com
    ServerName test.shivm07.shop
    ServerAlias test.shivm07.shop

    DocumentRoot /var/www/html/hostel-management-project-PHP/hostel
    <Directory /var/www/html/hostel-management-project-PHP/hostel>
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
        DirectoryIndex index.php index.html
    </Directory>

    ErrorLog ${APACHE_LOG_DIR}/your_project_error.log
    CustomLog ${APACHE_LOG_DIR}/your_project_access.log combined

    <FilesMatch \.php$>
        SetHandler application/x-httpd-php
    </FilesMatch>
</VirtualHost>

```

## Login details
```
Login Details for admin : admin/Test@1234
Login Details for user : test@gmail.com/Test@123
```

##For User

```
Login Details for user: 
Username: test@gmail.com
Password: Test@123
```

## For Admin Panel

```
Open Your browser put inside browser “http://localhost/library/admin”
Login Details for admin : 
Username: admin
Password:Test@123
```
