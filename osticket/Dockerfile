FROM php:8.1-fpm-alpine

RUN docker-php-ext-install mysqli

COPY php.ini /usr/local/etc/php/php.ini
COPY upload /var/www/html