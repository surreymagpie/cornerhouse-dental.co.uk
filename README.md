# Codebase for cornerhouse-dental.co.uk

This is the codebase for [Cornerhouse Dental Practice](www.cornerhouse-dental.co.uk)

## Local environment

Development using docker using my [surreymagpie/php-apache](https://www.github.com/surreymagpie/php-apache) image.

The docker environment can be initiated with:

`docker-compose up -d`

then the site is available at [http://localhost:8080](http://localhost:8080).

## Installation

The site can be reinstalled using:

```bash
docker-compose exec -u www-data php bash -c 'drush site:install minimal --db-url="mysql://drupal:drupal@db:3306/drupal" --site-name="Cornerhouse Dental Practice" -y'
```
