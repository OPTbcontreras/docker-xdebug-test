# docker-xdebug-test

Testing Xdebug and php-fpm within Docker.

## Setup

Edit `docker-compose.yaml` and set the `XDEBUG_CONFIG` env var to point to your Docker host's IP.

In your OS's hosts file, point `php-docker.local` to your Docker host (most likely 127.0.0.1).

## Run

```sh
docker-compose up -d
```

Head to http://php-docker.local:8080/ or http://php-docker.local:8080/phpinfo.php

Xdebug is configured on port 9004.
