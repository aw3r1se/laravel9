# Laravel 9 (Laradock + Breeze) Deploy
## Clone
 - git clone --recurse-submodules {url}
## Installation
 - cd {app_name}
 - cp .env.example .env
 - cd laradock
 - cp .env.example .env
 - laradock/.env:42 switch PHP_VERSION from 7.4 to 8.1
 - docker-compose build php-fpm nginx mysql adminer
 - docker-compose up -d nginx mysql adminer
 - docker-compose exec workspace bash
### Inside the container workspace
 - composer install
 - php artisan key:generate
 - .env:14 set a correct db_name
 - php artisan migrate
 - php artisan storage:link
 - chmod -R 777 storage
 - npm install
 - npm run dev

