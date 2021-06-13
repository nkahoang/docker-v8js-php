# Docker files for PHP with V8JS built-in

The repo available for the official debian-based PHP-FPM and official Wordpress-based PHP-FPM. This uses multi-stage docker build to minimise the image.

Now supporting V8 version 8.9 on PHP 7.3/7.4. PHP 8.0 is not yet supported with current [phpv8](https://github.com/phpv8/) project.

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
