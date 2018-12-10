FROM alpine:latest

MAINTAINER Isam Balushi

RUN apk --update \
    add apache2 \
    && rm -f /var/cache/apk/* \
    && mkdir /run/apache2

COPY www/ /var/www/localhost/htdocs

CMD [ "/usr/sbin/httpd", "-D", "FOREGROUND"]
