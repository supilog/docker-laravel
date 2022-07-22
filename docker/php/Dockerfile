FROM php:7.4-fpm

COPY ./conf/php.ini /etc/php.ini

COPY --from=composer:2.2 /usr/bin/composer /usr/bin/composer

ENV COMPOSER_ALLOW_SUPERUSER 1
ENV COMPOSER_HOME /composer

RUN apt-get update
RUN apt-get -y install --no-install-recommends git unzip libzip-dev libicu-dev
#libonig-devRUN
RUN apt-get -y install mariadb-client
RUN rm -rf /var/lib/apt/lists/*
RUN docker-php-ext-install intl pdo_mysql zip bcmath

WORKDIR /usr/local/nginx/vhosts/laravel.local.com/htdocs
