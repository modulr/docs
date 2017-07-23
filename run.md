# Run

#### Run migrations

```bash
~/modulr-laravel$ php artisan migrate
```

#### Run seeders _optional_

> NOTE: Seeds create 10 users

```bash
~/modulr-laravel$ php artisan db:seed
```

#### Compiling Assets (Laravel Mix)

```bash
// Run all Mix tasks...
~/modulr-laravel$ npm run dev

// Run all Mix tasks and minify output...
~/modulr-laravel$ npm run production

// Watching Assets For Changes
~/modulr-laravel$ npm run watch
```

#### Run serve

Local Development Server

If you have PHP installed locally and you would like to use PHP's built-in development server to serve your application, you may use the serve Artisan command. This command will start a development server at http://localhost:8000

```bash
~/modulr-laravel$ php artisan serve
```
