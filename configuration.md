# Configure

## Generate .env

```bash
~/modulr-laravel$ cp .env.example .env
```


## Generate APP_KEY

```bash
~/modulr-laravel$ php artisan key:generate
```


## Generate Symbolic link to Storage

```bash
~/modulr-laravel$ php artisan storage:link
```


## Create Data Base

```bash
~/modulr-laravel$ mysql -u{user} -p{password}
~/modulr-laravel$ create database modulr_laravel;
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
