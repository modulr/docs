# News

![news](http://modulr.io/img/modules/news.png)


## Backend

#### Migration

File: [database/migrations/2017_07_05_210219_create_news_table.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/database/migrations/2017_07_05_210219_create_news_table.php)

```php
$table->increments('id');
$table->text('title')->nullable();
$table->text('video')->nullable();
$table->integer('type');
$table->integer('user_id')->unsigned();
$table->foreign('user_id')->references('id')->on('users');
$table->json('likes');
$table->timestamps();
$table->softDeletes();
```

#### Models

File: [app/News.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/app/News.php)

#### Routes

File: [routes/web.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/routes/web.php)

```php
// News
    Route::get('/news', 'NewsController@index');
    Route::get('/news/all', 'NewsController@all');
    Route::post('/news/store', 'NewsController@store');
    Route::delete('/news/destroy/{id}', 'NewsController@destroy');
    Route::post('/news/like/{id}', 'NewsController@like');
    Route::post('/news/upload/temp', 'NewsController@uploadTemp');
```

#### Controllers

File: [app/Http/Controllers/NewsController.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/app/Http/Controllers/NewsController.php)

#### Views

File: [resources/views/news.blade.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/resources/views/news.blade.php)

## Frontend

#### Components

Folder: [resources/assets/js/components/news](https://github.com/modulr/laravel-scaffold-v1/tree/master/resources/assets/js/components/news)

File: [resources/assets/js/components/news/News.vue](https://github.com/modulr/laravel-scaffold-v1/tree/master/resources/assets/js/components/news/News.vue)

#### Sass

File: [resources/assets/sass/_news.scss](https://github.com/modulr/laravel-scaffold-v1/blob/master/resources/assets/sass/_news.scss)
