# Laravel 9 (Laradock + Breeze)
## Installation
 - cp .env.example .env
 - cd laradock
 - cp .env.example .env
 - docker-compose build php-fpm nginx mysql adminer
 - docker-compose up -d nginx mysql adminer
 - docker-compose exec workspace bash
### Inside the container workspace
 - composer install
 - php artisan key:generate
 - php artisan migrate
 - php artisan storage:link
 - chmod -R 777 storage
 - npm install
 - npm run dev

