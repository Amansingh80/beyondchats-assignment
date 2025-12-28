# Laravel Backend

## Setup Instructions

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

## Features
- Article scraping from BeyondChats blog
- CRUD APIs for article management
- MySQL database integration

## API Endpoints
- GET /api/articles
- GET /api/articles/{id}
- POST /api/articles
- PUT /api/articles/{id}
- DELETE /api/articles/{id}