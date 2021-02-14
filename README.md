# Laravel email notification example

## Installation

Clone the repo
```php
git clone https://github.com/teacoders/laravel-notification-example.git
```

Go to project directory
```php
cd laravel-notification-example
```
Install all composer dependencies
```php
composer install
```

Install all npm dependencies and compile them
```php 
npm install && npm run dev
```

copy .env.example to .env
```php
cp .env.example .env
```

Generate keys for your project
```php
php artisan key:generate
```

Change into following enviroment variable
```php
DB_CONNECTION=your_db_connection
DB_HOST=db_host_name
DB_PORT=db_port
DB_DATABASE=db_name
DB_USERNAME=db_user_name
DB_PASSWORD=db_password

QUEUE_CONNECTION=database // You can use another queue driver if you want and if you don't want to use the queue then don't change it and don't run any commands related to the queue

// add mailtrap or other mail service credentials
MAIL_DRIVER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=
MAIL_PASSWORD=
MAIL_ENCRYPTION=tls
```
And
```php
php artisan queue:table
php artisan migrate
php artisan serve
php artisan queue:work
```

## Credits

- [All Contributors](../../contributors)