# Docker files for PHP with V8JS built-in

The repo available for the official debian-based PHP-FPM and official Wordpress-based PHP-FPM. This uses multi-stage docker build to minimise the image.

Currently supporting V8 version 7.9 (as V8JS is not compatible with V8 v8+ yet) on PHP 7.3/7.4.

Docker Hub: https://hub.docker.com/r/nkahoang/docker-v8js-php

Wordpress images:
```bash
# 7.4
docker pull nkahoang/docker-v8js-php:wordpress5-php7.4-fpm-v8js7.9
# 7.3
docker pull nkahoang/docker-v8js-php:wordpress5-php7.3-fpm-v8js7.9
```

PHP-FPM images:
```bash
# 7.4
docker pull nkahoang/docker-v8js-php:php7.4-fpm-v8js7.9
# 7.3
docker pull nkahoang/docker-v8js-php:php7.3-fpm-v8js7.9
```

Examples docker-compose.yml usage (with Wordpress / MariaDB / Nginx) is in `/examples/wordpress` folder.
