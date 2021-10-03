FROM php:7.4.3-fpm

RUN apt-get -y install libmcrypt-dev

RUN apt-get install zlib1g-dev
RUN apt-get install libpng-dev
RUN apt-get install libzip-dev

RUN apt-get install libldb-dev libldap2-dev

RUN docker-php-ext-install pdo_mysql

RUN docker-php-ext-install bcmath

RUN docker-php-ext-install pcntl

RUN docker-php-ext-install gd

RUN docker-php-ext-install ldap

RUN docker-php-ext-install zip


cd /mnt/mongodb-1.10.0 \ phpize \ ./configure  \ make && make install