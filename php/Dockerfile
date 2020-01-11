FROM devilbox/php-fpm:7.3-work
ADD php.ini /usr/local/etc/php/conf.d/zzz-custom.ini
ADD empty_php.ini /usr/local/etc/php/conf.d/php.ini
#USER www-data
WORKDIR /var/www/html/default
EXPOSE 9000
CMD ["php-fpm"]