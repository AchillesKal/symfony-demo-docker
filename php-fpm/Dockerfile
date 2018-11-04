FROM php:7-fpm

RUN usermod -u 1000 www-data

RUN apt-get update && apt-get install -y \
  apt-utils \
  g++ \
  zlib1g-dev \
  libicu-dev


RUN docker-php-ext-install intl

EXPOSE 9000

CMD ["php-fpm"]