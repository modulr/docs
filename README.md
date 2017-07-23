# modulr-laravel

## Table of Contents

* [Install](#install)
* [Configure](#configure)
* [Community](#community)
* [Credits](#credits)
* [License](#license)

## Install

Clone repository

```
$ git clone https://github.com/modulr/modulr-laravel.git
```

Enter to folder

```
$ cd modulr-laravel
```

Install dependencies

```
// Composer
~/modulr-laravel$ composer install

// npm
~/modulr-laravel$ npm install
```

##

## Configure

Create .env file

```
~/modulr-laravel$ cp .env.example .env
```

Generate APP_KEY

```
~/modulr-laravel$ php artisan key:generate
```

Create Data Base

```
~/modulr-laravel$ mysql -u{user} -p{password}
~/modulr-laravel$ create database modulr_laravel
```

Configure .env file

```
// Add database config params
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=modulr_laravel
DB_USERNAME=user
DB_PASSWORD=password

// Add broadcasting config params
BROADCAST_DRIVER=pusher

PUSHER_APP_ID=pusher_id
PUSHER_APP_KEY=pusher_key
PUSHER_APP_SECRET=pusher_secret
```

Run migrations

```
~/modulr-laravel$ php artisan migrate
```

Run seeders _ \_optional_ \_

> NOTE: Seeds create 10 users and 3 news for user

```
~/modulr-laravel$ php artisan db:seed
```

Build js, css & assets

> NOTE: Developer mode

```
~/modulr-laravel$ npm run dev
```

Run serve

```
~/modulr-laravel$ php artisan serve
```

## Community

* Join [the official Slack room](https://modulr.slack.com/).
* Implementation help may be found at Stack Overflow \(tagged [`modulr`](http://stackoverflow.com/questions/tagged/modulr)\).

## Credits

* [@alfredobarron](https://github.com/alfredobarron)
* [@deleonn](https://github.com/deleonn)
* [@EduardoDArellano](https://github.com/EduardoDArellano)

## License

The [MIT©](https://github.com/modulr/modulr/blob/master/LICENSE) License 2017 - Modulr.
