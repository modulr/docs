# Contacts

![contacts](http://modulr.io/img/modules/contacts.png)


## Backend

#### Migration

File: [database/migrations/2014_10_12_000000_create_users_table.php](https://github.com/modulr/modulr-laravel/blob/master/database/migrations/2014_10_12_000000_create_users_table.php)

```php
$table->increments('id');
$table->string('name');
$table->string('email')->unique();
$table->string('password');
$table->string('avatar');
$table->boolean('active')->default(true);
$table->rememberToken();
$table->timestamps();
$table->softDeletes();
```

#### Models

File: [app/User.php](https://github.com/modulr/modulr-laravel/blob/master/app/User.php)

#### Routes

File: [routes/web.php](https://github.com/modulr/modulr-laravel/blob/master/routes/web.php)

```php
// Contacts
Route::get('/contacts', 'ContactsController@index');
Route::get('/contacts/all', 'ContactsController@all');
```

#### Controllers

File: [app/Http/Controllers/ContactsController.php](https://github.com/modulr/modulr-laravel/blob/master/app/Http/Controllers/ContactsController.php)

#### Views

File: [resources/views/contacts.blade.php](https://github.com/modulr/modulr-laravel/blob/master/resources/views/contacts.blade.php)

## Frontend

#### Components

Folder: [resources/assets/js/components/contacts](https://github.com/modulr/modulr-laravel/tree/master/resources/assets/js/components/contacts)

File: [resources/assets/js/components/Contacts.vue](https://github.com/modulr/modulr-laravel/tree/master/resources/assets/js/components/Contacts.vue)

#### Sass

File: [resources/assets/sass/_contacts.scss](https://github.com/modulr/modulr-laravel/blob/master/resources/assets/sass/_contacts.scss)
