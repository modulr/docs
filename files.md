# Files

![files](http://modulr.io/img/modules/files.png)


## Backend

#### Migration

File: [database/migrations/2017_07_12_233302_create_files_table.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/database/migrations/2017_07_12_233302_create_files_table.php)

```php
$table->increments('id');
$table->text('name');
$table->text('basename')->nullable();
$table->string('extension')->nullable();
$table->text('description')->nullable();
$table->boolean('favorite')->default(false);
$table->integer('parent_id')->default(0);
$table->integer('type')->default(1); // 1.File, 2.Folder
$table->integer('user_id')->unsigned();
$table->foreign('user_id')->references('id')->on('users');
$table->timestamps();
$table->softDeletes();
```

#### Models

File: [app/File.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/app/File.php)

#### Routes

File: [routes/web.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/routes/web.php)

```php
// Files
    Route::get('/file/byUser/{parentId?}', 'FileController@byUser');
    Route::post('/file/store', 'FileController@store');
    Route::put('/file/update/{id}', 'FileController@update');
    Route::delete('/file/destroy/{id}', 'FileController@destroy');
    Route::get('/files/{folderId?}', 'FileController@view');
```

#### Controllers

File: [app/Http/Controllers/FileController.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/app/Http/Controllers/FileController.php)

#### Views

File: [resources/views/files.blade.php](https://github.com/modulr/laravel-scaffold-v1/blob/master/resources/views/files.blade.php)

## Frontend

#### Components

Folder: [resources/assets/js/components](https://github.com/modulr/laravel-scaffold-v1/tree/master/resources/assets/js/components/files)

File: [resources/assets/js/components/Tasks.vue](https://github.com/modulr/laravel-scaffold-v1/tree/master/resources/assets/js/components/files/Files.vue)

#### Sass

File: [resources/assets/sass/_files.scss](https://github.com/modulr/laravel-scaffold-v1/blob/master/resources/assets/sass/_files.scss)
