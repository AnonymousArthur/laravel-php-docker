# Laravel PHP Docker Image

## About
This Dockerfile builds an image to support Laravel to run.

## Prerequisite
* Linux or macOS
* Docker CE Edge build. Downloads: [mac](https://store.docker.com/editions/community/docker-ce-desktop-mac) [ubuntu](https://docs.docker.com/v17.12/install/linux/docker-ce/ubuntu/)

## What's inside the box
* Debian stretch
* PHP-FPM 7.2
* PHP extensions: mongodb, postgres, pdo and more...
* Xdebug
* Composer
* NPM
* NodeJS

Note: MySQL PDO is not supported in this image

## Installation
Make sure you're at this Dockerfile's root.
```bash
docker build -t laravel-php .
```

## Customizations
### PHP
If you want to customize `php.ini`, place your `php.ini` in `/usr/local/etc/php/`.

## TODO List:
* Use Alpine Linux instead of Debian to reduce image size.
* Support MySQL PDO
* ...