FROM php:7.1-fpm

RUN pecl install xdebug-2.5.5 && \
    docker-php-ext-enable xdebug   

RUN touch /var/log/xdebug.log && chown www-data:www-data /var/log/xdebug.log 

COPY php.ini /usr/local/etc/php/php.ini
COPY xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini
