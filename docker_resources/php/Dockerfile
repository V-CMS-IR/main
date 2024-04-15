FROM php:8.3-fpm-bullseye


RUN apt update && apt install -y zip unzip git libpng-dev 




RUN docker-php-ext-install bcmath pdo_mysql gd
#RUN docker-php-ext-install soap
#RUN docker-php-ext-install zip
#RUN docker-php-ext-install readline xdebug


#RUN docker-php-ext-install ldap   memcached  msgpack   pcov


RUN curl -sLS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ --filename=composer 

#RUN apt-get update && apt-get install -y mysql-client

USER root

CMD php-fpm -R