## Clone this repository
```
  git clone https://github.com/shivm04/library-management-project-php.git
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
  CREATE DATABASE library;

  Import the hostel.sql file into the hostel database
  mysql -u root -p library < library.sql

```

## Chnage the permission of the files 
```
chmod -R 755 library-management-project-php/ library-management-project-php/*
chown -R www-data:root library-management-project-php/* library-management-project-php/
```

## Change the database Credentials in the configuration file 
```
   library-management-project-php/library/includes
```

## Create a config file for the apache to host our website 

```
<VirtualHost *:80>
    ServerAdmin webmaster@your_domain.com
    ServerName test1.shivm07.shop
    ServerAlias test1.shivm07.shop

    DocumentRoot /var/www/html/library-management-project-php/library
    <Directory /var/www/html/library-management-project-php/library>
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
