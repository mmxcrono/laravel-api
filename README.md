# Laravel API

## Docker Setup

1. Install Docker Desktop on Windows
2. Enable WSL2 mode in settings

## Docker Compose

Run `docker-compose build`
Run `docker-compose up -d`
Run `docker-compose exec app composer install`
Run `docker-compose exec app php artisan key:generate`
Run `docker-compose exec app php artisan migrate`

## Launch

Open a browser to http://localhost:8000
