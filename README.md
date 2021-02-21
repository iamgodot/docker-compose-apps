# Docker Compose Apps

## Intro

This repo keeps a collection of docker compose config files for different self-hosting apps.

## Usage

1. Clone the repo to your server, and copy the app folder to the right place.

2. Setup `.env` file accordingly.

3. Make sure docker and docker-compose are properly installed, then run `docker-compose run -d` to start the service.

4. To stop the service, run `docker-compose stop`.

5. To remove the service, run `docker-compose kill && docker-compose rm`.

## Apps

### wordpress

Two additional config files are intended to solve the custom issues: 

- [For Nginx](wordpress/nginx-conf/custom_settings.conf)  

- [For Php](wordpress/php-conf/custom_settings.ini)

References from Github: 

- [Docker-compose.yml and client_max_body_size](https://github.com/nginx-proxy/nginx-proxy/issues/690)

- [Increase PHP file upload limit](https://github.com/docker-library/wordpress/issues/10)
