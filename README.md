# umami-docker-compose
A simple docker compose configuration for Umami. It uses Traefik to route traffic by domain. 

## Configuration
The only configuration, that needs to be set, is located in .env:
```
COMPOSE_PROJECT_NAME=umami
DOMAIN=umami.example.net
```
The DOMAIN must be set to your domain, where umami will be accessed.

## Start Umami and access

Traefik needs to be running, so that Umami is reachable at the domain specified in `.env`. To start Umami, just execute `docker-compose start -d`.

Traefik will automatically configure ssl certificates etc.



