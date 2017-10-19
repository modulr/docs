# Install Requirements


## Install Linux



## Install Apache





!> NOTE: enabled mod_rewrite virtual host

```
<Directory "/var/www/html/laravel/public">
    Allowoverride All
</Directory>
```



## Install MySQL

```bash
$ sudo apt install php7.0-mysql
```


## Install PHP



#### Install PHP Requirements

PHP >= 7.0.0

OpenSSL PHP Extension `enabled default on php 7`

PDO PHP Extension `enabled default on php 7`

Tokenizer PHP Extension `enabled default on php 7`

Install Mbstring PHP Extension

`$ sudo apt-get install php7.0-mbstring`

Install XML PHP Extension

`$ sudo apt-get install php7.0-xml`

Install GD module for PHP

`$ sudo apt-get install php7.0-gd`


## Install Git

```bash
$ sudo apt-get install git
```



## Install composer

```bash
$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
$ php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ php composer-setup.php
$ php -r "unlink('composer-setup.php');"

// Install globally as a system wide executable
$ sudo mv composer.phar /usr/local/bin/composer
```

> NOTE: Composer requiere unzip

#### Install unzip

`$ sudo apt-get install unzip`



## Install Node & NPM

```bash
$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```
