FROM jcomack/php5cli

MAINTAINER "Jimmy Comack" <jimcom89@gmail.com>

WORKDIR /tmp

RUN apt-get update -y && \
    apt-get install -y curl git php5-mcrypt php5-gd && \
    curl -sS https://getcomposer.org/installer | php && \
    mv composer.phar /usr/local/bin/composer && \
    apt-get remove --purge curl -y && \
    apt-get clean

RUN mkdir -p /data/www
VOLUME ["/data"]
WORKDIR /data/www

ENTRYPOINT ["composer"]
CMD ["--help"]
