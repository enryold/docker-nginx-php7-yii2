# docker-nginx-php7-yii2
Docker image based on phusion/base-image with nginx php7-fpm, configured to use yii2 project


Basic Usage.

```
FROM enryold/nginx-php7-fpm-yii2

COPY . /var/www

RUN chmod -R 777 /var/www/assets
RUN chmod -R 777 /var/www/runtime
RUN chmod -R 777 /var/www/web/assets
RUN chmod -R 777 /var/www/tmp
