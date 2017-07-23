# Tasks

![tasks](http://modulr.io/img/modules/tasks.png)


## Backend

#### Migration

File: [database/migrations/2017_07_08_211240_create_tasks_table.php](https://github.com/modulr/modulr-laravel/blob/master/database/migrations/2017_07_08_211240_create_tasks_table.php)

```php
$table->increments('id');
$table->string('title');
$table->boolean('done')->default(false);
$table->integer('order');
$table->integer('user_id')->unsigned();
$table->foreign('user_id')->references('id')->on('users');
$table->timestamps();
$table->softDeletes();
```

#### Models

File: [app/Task.php](https://github.com/modulr/modulr-laravel/blob/master/app/Task.php)

#### Routes

File: [routes/web.php](https://github.com/modulr/modulr-laravel/blob/master/routes/web.php)

```php
//Tasks
    Route::get('/tasks', 'TaskController@view');
    Route::get('/task/byUser', 'TaskController@byUser');
    Route::post('/task/store', 'TaskController@store');
    Route::delete('/task/destroy/{id}', 'TaskController@destroy');
    Route::put('/task/markDone/{id}', 'TaskController@markDone');
    Route::put('/task/updateOrder', 'TaskController@updateOrder');
    Route::put('/task/editTask/{id}', 'TaskController@editTask');
```

#### Controllers

File: [app/Http/Controllers/TaskController.php](https://github.com/modulr/modulr-laravel/blob/master/app/Http/Controllers/TaskController.php)

#### Views

File: [resources/views/tasks.blade.php](https://github.com/modulr/modulr-laravel/blob/master/resources/views/tasks.blade.php)

## Frontend

#### Components

Folder: [resources/assets/js/components](https://github.com/modulr/modulr-laravel/tree/master/resources/assets/js/components)

File: [resources/assets/js/components/Tasks.vue](https://github.com/modulr/modulr-laravel/tree/master/resources/assets/js/components/Tasks.vue)

#### Sass

File: [resources/assets/sass/_tasks.scss](https://github.com/modulr/modulr-laravel/blob/master/resources/assets/sass/_tasks.scss)
