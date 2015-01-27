FROM debian:jessie

MAINTAINER "Jimmy Comack" <jimcom89@gmail.com>

# Install PHP-CLI
RUN apt-get update -y && \
    apt-get install php5-cli -y

ENTRYPOINT ["php"]
CMD ["--help"]
