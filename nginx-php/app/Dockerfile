FROM php:7.4.7-fpm

RUN apt-get update && apt-get install -y default-mysql-client libmcrypt-dev libcurl3-dev zip unzip \
    && docker-php-ext-install curl \
    && docker-php-ext-install pdo_mysql \
    && curl -sS https://getcomposer.org/installer | php \
    && mv composer.phar /usr/local/bin/composer

WORKDIR /var/www
