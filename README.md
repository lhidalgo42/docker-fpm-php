# Make your FPM-PHP fly on Alpine

## Overview

This is a Dockerfile/image to build a container for FPM-PHP.
Most of the regular needed modules (apcu, opcache, php-redis, etc.) are built in and configured like suggested on [php.net](https://secure.php.net/).

## Regular builds, automagically

[![Build Status](https://travis-ci.com/Hermsi1337/docker-fpm-php.svg?branch=master)](https://travis-ci.com/Hermsi1337/docker-fpm-php)  
Thanks to [Travis-CI](https://travis-ci.com/) this image is pushed weekly and creates new [tags](https://hub.docker.com/r/hermsi/alpine-fpm-php/tags/) if there are new versions available.

## Tags

For recent tags check [Dockerhub](https://hub.docker.com/r/hermsi/alpine-fpm-php/tags/).

* `7.4.0` `7.4`, `7`, `latest`, `stable`
* `7.3.6`,`7.3.5`,`7.3.4`, `7.3.3`, `7.3`
* `7.2.19`, `7.2.18`, `7.2.17`, `7.2.16`, `7.2`
* `7.1.30`, `7.1.29`, `7.1.28`, `7.1.27`, `7.1`
* `7.0.33`, `7.0` (`EOL`)

## Features

* intl
* zip
* soap
* mysqli
* pdo
* pdo_mysql
* pdo_pgsql
* mcrypt
* exif
* gd
* iconv
* xsl
* bcmath
* gmp
* php-redis
* memcached
* openssl
* opcache ([configuration reference](https://secure.php.net/manual/en/opcache.installation.php))
* apcu ([configuration reference](https://secure.php.net/manual/en/apcu.configuration.php))
* imagick
* ssh2 (< 7.3)
* ioncube
* mcrypt (< 7.2)

## Basic Usage

This Image is intended to be used along with an external webserver container like apache or nginx.
I personally prefer nginx over apache. If you are interested in how to setup nginx along with this fpm-php image, take a look at [my docker-compose files](https://github.com/Hermsi1337/docker-compose/blob/master/full_php_dev_stack/docker-compose.yml).