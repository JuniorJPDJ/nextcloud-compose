# Full stack Nextcloud docker-compose 

Stack:
- Nextcloud
- postgres
- nginx
- php-fpm
- cron

It already contains smb, imap and libreoffice support

The only thing you need to do is specify your postgresql db password in `postgres.env` file

This stack is not providing SSL by default and is ment to be put behind some sort of reverse proxy (eg. haproxy) with SSL termination

Based on:
- https://github.com/nextcloud/docker/blob/master/.examples/dockerfiles/full/fpm-alpine/Dockerfile
- https://github.com/nextcloud/docker/tree/master/.examples/docker-compose/insecure/postgres/fpm
- https://github.com/nextcloud/docker/tree/master/.examples/docker-compose/insecure/mariadb-cron-redis/fpm

