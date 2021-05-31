FROM php:8.0.6-apache
RUN curl -sS https://getcomposer.org/installer -o composer-setup.php
RUN php composer-setup.php --install-dir=/usr/local/bin --filename=composer
RUN cd /var/www/html
RUN apt-get update
RUN apt-get install zip unzip
RUN composer require symfony/apache-pack

