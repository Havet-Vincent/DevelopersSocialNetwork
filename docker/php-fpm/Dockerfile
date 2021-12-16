ARG PHP_VERSION
FROM php:${PHP_VERSION}-fpm

RUN apt-get update && docker-php-ext-install pdo_mysql

COPY --from=composer:2.1.14 /usr/bin/composer /usr/local/bin/composer

