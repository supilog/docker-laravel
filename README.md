# docker-laravel
## construction
### install
    git clone リポジトリ
    cd docker-laravel
    composer install
    cp -i .env.example .env
    php artisan key:generate
    docker compose up -d
    
    docker compose exec php bash
    php artisan migrate
    php artisan db:seed
    exit
### build & up
    docker compose build
    docker compose up -d
### down
    docker compose down
### shell
    docker compose exec nginx bash
    docker compose exec php bash
    docker compose exec mysql bash
