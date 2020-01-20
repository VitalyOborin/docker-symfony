# Docker-compose for Symfony project
## Description
Simple solution for fast run symfony application. Contains nginx, php_fpm, mysql, kafka and zookeeper. 
Currently using for my private symfony 5.0 project. Suitable **only for development**, not for production use.
## Run
Create directory, for example `docker`. In that directory run `git clone git@github.com:VitalyOborin/docker-symfony.git` . Correct paths: 

* In docker-compose.yml change path in `../sites/:/var/www/html/` to folder with projects
* In nginx/sites-allowed/default.conf change path `root /var/www/html/cart/public;` to your default site. /var/www/html/ is already mounted in docker-compose.yml.
 
Now you can run services:
`docker-compose up -d --build`. 
## Stop
`docker-compose down`
## Reload nginx configs
`docker exec -t nginx nginx -s reload`
## To-do
* PHP based on clean php-fpm with really used modules.
* nginx config for multiple sites