FROM php:7.0-apache
RUN a2enmod proxy
RUN a2enmod proxy_http
RUN a2enmod proxy_wstunnel
RUN a2enmod rewrite
COPY apache2.conf /usr/local/apache2/conf/httpd.conf
COPY 000-default.conf /etc/apache2/sites-enabled/000-default.conf

