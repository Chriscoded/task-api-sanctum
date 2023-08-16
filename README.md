# Laravel Sanctum API
- [Laravel Sanctum](https://laravel.com/docs/9.x/sanctum) for an authentication system
- [Postman](https://www.postman.com/) for our Laravel API
- [Database Client](https://tableplus.com/) to have a look inside our database

## Usage <br>
Setup the repository <br>
```
git clone https://github.com/Chriscoded/task-api-sanctum.git
cd laravel-sanctum-tutorial
composer install
cp .env.example .env 
php artisan key:generate
php artisan cache:clear && php artisan config:clear 
php artisan serve 
```

## Database Setup <br>
```
mysql;
create database laravel-sanctum-tutorial;
exit;
```


### Setup your database credentials in the ```.env``` file <br>
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel-sanctum-tutorial
DB_USERNAME={USERNAME}
DB_PASSWORD={PASSWORD}
```

### Sanctum
Before you can use Laravel Sanctum, you obviously need to make sure that you install it through Composer. Besides that, you should upblish the Sanctum configuration file as well.
```
composer require laravel/sanctum
php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider"
```

### Migrate tables
```
php artisan migrate
```

# links
<a href="https://laravel.com/"></a> 
<a href="https://laravel.com/docs/9.x/sanctum">Santum</a> 
