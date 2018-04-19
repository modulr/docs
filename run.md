# Run

## Run migrations

```bash
~/modulr-laravel$ php artisan migrate
```


## Run seeders

This seeder fill lists to database

```bash
~/modulr-laravel$ php artisan db:seed
```


## Run Faker Seeder _optional_

This seeder create 10 users to database

```bash
~/modulr-laravel$ php artisan db:seed --class=FakerSeeder
```

!> If exist someting error run this command


```bash
$ composert dumpautoload
```


## Compiling Assets (Laravel Mix)

```bash
// Watching Assets For Changes
~/modulr-laravel$ npm run watch

// Run all Mix tasks...
~/modulr-laravel$ npm run dev

// Run all Mix tasks and minify output...
~/modulr-laravel$ npm run production
```


## Run serve

Local Development Server

If you have PHP installed locally and you would like to use PHP's built-in development server to serve your application, you may use the serve Artisan command. This command will start a development server at [http://localhost:8000](http://localhost:8000)

```bash
~/modulr-laravel$ php artisan serve
```
