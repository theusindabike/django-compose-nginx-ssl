# django-compose-nginx-ssl

Here we have: 
1. an Django app 
2. with [Nginx](https://nginx.org/en/) as reverse proxy 
3. and [certbot](https://hub.docker.com/r/certbot/certbot/) helping to renew ssl certificate

Then, [docker-compose](https://docs.docker.com/compose/)

## Installation
Just replace:
1. <DJANGO_APP_NAME> in docker-compose.yaml file
2. Adjust variables in .env-sample

## Usage

```bash
docker-compose up --build
```
