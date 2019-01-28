FROM nginx:alpine

ARG GID=1000

RUN addgroup -g $GID rtorrent && \
addgroup nginx rtorrent && \
mkdir /rutorrent && \
chown -R nginx:nginx /rutorrent

WORKDIR /etc/nginx/conf.d

RUN rm default.conf

COPY rutorrent.conf .