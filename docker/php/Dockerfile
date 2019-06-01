FROM php:7.2-fpm

# Install Composer
RUN curl -s http://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
RUN apt-get update \
    && apt-get install -y \
        git \
        zip \
        unzip \
        vim

RUN apt-get update \
    && apt-get install -y libpq-dev \
    && docker-php-ext-install pdo_mysql pdo_pgsql