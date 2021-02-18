FROM php:8.0.2-fpm-alpine3.13

RUN apk add --no-cache ca-certificates \
    bash \
    git \
    nodejs=14.15.5-r0 \
    npm=14.15.5-r0 \
    sudo 

COPY docker/app/php.ini /usr/local/etc/php/conf.d/local.ini  

COPY . /var/www/app

WORKDIR /var/www/app

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

ENTRYPOINT [ "/var/www/app/docker/entrypoint.sh" ]