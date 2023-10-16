# Laravel API

This project will set up a Laravel API

-   Use argon2id for password hashing
-   Use Vue with Breeze for the UI
-   Use Sanctum for authentication

## Environment

See `.env.example` and copy to .env, replacing as needed.

## Node Setup

1. Run `npm ci && npm run build`
2. Run `npm run dev`

## Docker Setup

1. Install Docker Desktop on Windows
2. Enable WSL2 mode in settings

## Docker Compose

Run the following commands one at a time

```sh
docker-compose build
docker-compose up -d
docker exec app composer install
docker exec app php artisan key:generate
docker exec app php artisan migrate
docker exec app php artisan test
```

## Launch

Open a browser to http://localhost:8000

## Make Model

1. Run

```sh
docker-compose exec app php artisan make:model
```

2. Provide model name
3. Choose file creation options

## Migrations

### Migrate and run seeders

Run

```sh
docker-compose exec app php artisan migrate --seed
```

### Rollback

Run

```sh
docker-compose exec app php artisan migrate:rollback
```

## Make Resource TaskResource

Run

```sh
docker-compose exec app php artisan make:resource TaskResource
```

## Make Controller

1. Run

```sh
docker-compose exec app php artisan make:controller
```

2. Choose type of controller

## Run "inspire" Command

Run

```sh
docker-compose exec app php artisan inspire
```
