# todo use clean php-fpm
FROM devilbox/php-fpm:7.3-work
#USER www-data
# disable unsed PHP modules
RUN rm -f /usr/local/etc/php/conf.d/docker-php-ext-calendar.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-enchant.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-gmp.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-imagick.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-ldap.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-interbase.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-memcached.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-memcache.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-msgpack.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-phalcon.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-pgsql.ini \
    /usr/local/etc/php/conf.d/docker-php-ext-uploadprogress.ini
WORKDIR /var/www/html/
EXPOSE 9000
CMD ["php-fpm"]