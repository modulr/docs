# Configure

## Generate .env

```bash
~/laravel-scaffold-v1$ cp .env.example .env
```


## Generate APP_KEY

```bash
~/laravel-scaffold-v1$ php artisan key:generate
```


## Generate Symbolic link to Storage

```bash
~/laravel-scaffold-v1$ php artisan storage:link
```


## Create Data Base

```bash
~/laravel-scaffold-v1$ mysql -u{user} -p{password}
~/laravel-scaffold-v1$ create database modulr_laravel;
```


## Database config params

```
// .env

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=modulr_laravel
DB_USERNAME=user
DB_PASSWORD=password
```


## Broadcasting config params

```
// .env file

BROADCAST_DRIVER=pusher
PUSHER_APP_ID=pusher_id
PUSHER_APP_KEY=pusher_key
PUSHER_APP_SECRET=pusher_secret
```
