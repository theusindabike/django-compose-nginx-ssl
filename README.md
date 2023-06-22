# django-compose-nginx-ssl

Here we have: 
1. an Django app 
2. with [Nginx](https://nginx.org/en/) as reverse proxy 
3. and [certbot](https://hub.docker.com/r/certbot/certbot/) helping to renew ssl certificate
4. Orchestrated by [docker compose](https://docs.docker.com/compose/)

## Installation
Just replace:
1. <DJANGO_APP_NAME> in docker-compose.yaml file
2. Adjust variables in .env-sample

## Usage

```bash
docker compose up --build
```

## Setup Certbot (SSL)
Assuming that you have you app running (e.g. on a AWS EC2):

- To init:
```
docker compose run --rm certbot /opt/certify-init.sh
```

- To renew: 
```
docker compose run --rm certbot sh -c "certbot renew"
```
