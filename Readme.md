# Requirements

- Composer
- Docker
  - docker-compose

## Installation

- Run `composer install`
- Go to the docker configuration folder you want to start and run `docker-compose up -d` to start the instance
- Use `docker-compose stop` to kill it again

### Ports
- PHP 5.6: 8500
- PHP 7.0 & NginX & MariaDB: 8701
- PHP 7.0 & NginX & MySQL: 8702
- PHP 7.0 & Apache & MySQL: 8703
- PHP 7.0 & Apache & MariaDB: 8704

To have the fastest experience, follow the installation instructions on https://github.com/moorscode/wp-multi-object-cache/ in combination with the `./docker/fastest/` docker-compose configuration.
This will use Redis and Memcache for Object Caching,

- PHP 7.0 & Redis & Memcached & NginX & MariaDB: 8700 (requires https://github.com/moorscode/wp-multi-object-cache/)
