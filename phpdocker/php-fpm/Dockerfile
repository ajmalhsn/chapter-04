FROM phpdockerio/php72-fpm:latest
WORKDIR "/application"
#INSTALL selected extensions and other stuff
RUN apt-get update \
	&& apt-get -y --no-install-recommends install php7.2-mysql && libmcrypt-dev \ && apt-get clean && docker-php-ext install pdo_mysql; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*/usr/share/doc/*
