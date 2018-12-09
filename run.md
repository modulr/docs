# Run

## Run migrations

```bash
~/laravel-scaffold-v1$ php artisan migrate
```


## Run seeders

This seeder fill lists to database

```bash
~/laravel-scaffold-v1$ php artisan db:seed
```


## Run Faker Seeder _optional_

This seeder create 10 users to database

```bash
~/laravel-scaffold-v1$ php artisan db:seed --class=FakerDataSeeder
```


## Compiling Assets (Laravel Mix)

```bash
// Watching Assets For Changes
~/laravel-scaffold-v1$ npm run watch

// Run all Mix tasks...
~/laravel-scaffold-v1$ npm run dev

// Run all Mix tasks and minify output...
~/laravel-scaffold-v1$ npm run production
```


## Run serve

Local Development Server

If you have PHP installed locally and you would like to use PHP's built-in development server to serve your application, you may use the serve Artisan command. This command will start a development server at [http://localhost:8000](http://localhost:8000)

```bash
~/laravel-scaffold-v1$ php artisan serve
```
