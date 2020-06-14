# WordPress Bootstrap

## INTRO

This repo keeps a handy copy of configuration and script files for bootstrapping of WordPress with docker-compose. And it's basically from [how-to-install-wordpress-with-docker-compose](https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-docker-compose).

Also, to solve the custom configuration issue for Nginx and PHP, I also add another two files: 

- [custom_settings.conf](./nginx-conf/custom_settings.conf)  

- [custom_php_configs.ini](./custom_php_configs.ini)

The idea comes from discussions of relative Github issues: [docker-compose.yml and client_max_body_size](https://github.com/nginx-proxy/nginx-proxy/issues/690) & [Increase PHP file upload limit](https://github.com/docker-library/wordpress/issues/10)

---

## USAGE

1. Read [how-to-install-wordpress-with-docker-compose](https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-docker-compose) first, then clone this repo to your server.

2. Replace `example.com` in [docker-compose.yml](./docker-compose.yml) and [nginx.conf](./nginx-conf/nginx.conf) with your own domain.

3. Update `WD_DIR` in [ssl_renew.sh](./ssl_renew.sh).

4. Use docker-compose to deploy WordPress.

---

## TODO

- [ ] The whole thing will be packed into an Ansible playbook in the future for time saving.
