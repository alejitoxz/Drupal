# Drupal 9

## Pre-requisits

 - Install docker

## Install environment
 - Go to main folder and execute `docker-compose build`
  - After that execute `docker-compose up -d`
  - To install the drupal environment you should go inside to the php container for that you can use: `docker-compose exec php-app bash`.
  - Inside the container on the *html* folder execute: `php -d memory_limit=-1 /usr/local/bin/composer install`.

## Install Drupal

To install Drupal you can go directly to the url and use Drupal intalation interface, also you can use a drush comand like this: `drush si standard --account-name=admin --account-pass=admin --db-url=mysql://root:root@database-app/drupal -y`

