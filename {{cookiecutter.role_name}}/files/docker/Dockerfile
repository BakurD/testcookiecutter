FROM php:8.2.5-fpm

RUN apt-get update && apt-get install -y \
    libsocket-perl

RUN docker-php-ext-install pdo mysqli pdo_mysql sockets

COPY php.ini /usr/local/etc/php/

WORKDIR /var/www/html


EXPOSE 9000


CMD ["php-fpm"]
