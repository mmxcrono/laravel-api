# Laravel API

## Docker Setup

1. Install Docker Desktop on Windows
2. Enable WSL2 mode in settings

## Docker Compose

1. Run `docker-compose build`
2. Run `docker-compose up -d`
3. Run `docker-compose exec app composer install`
4. Run `docker-compose exec app php artisan key:generate`
5. Run `docker-compose exec app php artisan migrate`

## Launch

Open a browser to http://localhost:8000


## Make Model

1. Run `docker-compose exec app php artisan make:model`
2. Provide model name
3. Choose file creation options

## Migrations

### Migrate and run seeders

Run `docker-compose exec app php artisan migrate --seed`

### Rollback

Run `docker-compose exec app php artisan migrate:rollback`

## Make Resource

Run `docker-compose exec app php artisan make:resource TaskResource`

## Make Controller

1. Run `docker-compose exec app php artisan make:controller`
2. Choose type of controller
