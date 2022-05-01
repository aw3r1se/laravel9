# Laravel 9 (Laradock + Breeze)
## Clone
 - git clone --recurse-submodules {url}
## Installation
 - cd {app_name}
 - cp .env.example .env
 - cd laradock
 - cp .env.example .env
 - .env:42 switch PHP_VERSION from 7.4 to 8.1
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

