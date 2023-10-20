FROM php:5.6.19-fpm-alpine
ENV TZ=Asia/Shanghai
COPY php-fpm/php-timezone.ini /usr/local/etc/php/conf.d/
RUN chmod 644 /usr/local/etc/php/conf.d/php-timezone.ini
RUN docker-php-ext-install mysqli pdo pdo_mysql
RUN docker-php-ext-install mysql
RUN docker-php-ext-install sockets
RUN docker-php-ext-enable mysql mysqli sockets

