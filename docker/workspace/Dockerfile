FROM php:7.4.9-zts-alpine3.12

WORKDIR /workspace

RUN apk add bash libzip-dev

RUN docker-php-ext-install zip

RUN curl -s https://getcomposer.org/installer | php


RUN mv composer.phar /usr/local/bin/composer
RUN composer global require laravel/installer


