FROM php:7.4.8-fpm-alpine3.12 

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/bin/

RUN install-php-extensions pdo_pgsql

# required by smarty
RUN mkdir templates_c 
