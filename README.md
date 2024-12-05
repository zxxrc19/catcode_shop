# laravel new name_project 

# composer update

# APP_URL=127.0.0.1:8000

# php artisan storage:link

# FILESYSTEM_DISK=public

# in phpunit.xml 
<env name="DB_DATABASE" value="shop_test"/>
<env name="DB_USERNAME" value="root"/>
<env name="DB_PASSWORD" value="ServBay.dev"/>

# in AppServiceProvider.php
use Illuminate\Database\Eloquent\Model;
use Illuminate\Support\ServiceProvider;
use Illuminate\Support\Facades\DB;


Model::preventLazyLoading(!app()->isProduction());
Model::preventSilentlyDiscardingAttributes(!app()->isProduction());
DB::whenQueryingForLongerThan(500, function (Connection $connection, QueryExecuted $event) {
    // 
});

# composer require barryvdh/laravel-debugbar --dev 

# composer require laravel/telescope

# php artisan telescope:install

# php artisan migrate 

# npm i 

# npm i -D tailwindcss

# npm i @tailwindcss/line-clamp