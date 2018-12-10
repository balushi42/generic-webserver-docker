FROM alpine:latest

MAINTAINER Isam Balushi

RUN apk --update \
    add apache2 \
    && rm -f /var/cache/apk/* \
    && mkdir /run/apache2

CMD [ "/usr/sbin/httpd", "-D", "FOREGROUND"]
