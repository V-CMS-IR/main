FROM php:fpm-bullseye


RUN apt update && apt install -y zip unzip git libpng-dev

RUN curl -sLS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ --filename=composer 

#RUN apt-get update && apt-get install -y mysql-client