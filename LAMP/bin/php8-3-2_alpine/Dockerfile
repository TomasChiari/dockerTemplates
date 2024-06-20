FROM php:8.2.20-apache-bookworm

# Disable window manager
ARG DEBIAN_FRONTEND=noninteractive

# update repos debian
RUN apt-get update

# install php extencions
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install pdo
RUN docker-php-ext-install pdo_mysql

# expose php port
EXPOSE 80 