FROM php:5.6.40-fpm-alpine3.8

ARG GID=1000

RUN addgroup -g $GID rtorrent && \
addgroup www-data rtorrent && \
mkdir /rutorrent /rtorrent && \
chown -R www-data:www-data /rutorrent