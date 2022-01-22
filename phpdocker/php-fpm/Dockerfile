FROM phpdockerio/php72-fpm:latest
# Add a new user "john" with user id 8877
#RUN useradd -u 8877 gitpod
# Change to non-root privilege
#USER gitpod

WORKDIR "/application"
# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install php7.2-mysq libmcrypt-dev \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
    