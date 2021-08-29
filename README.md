<p align="center"><a href="https://teacoders.in" target="_blank"><img src="https://teacoders.in/images/basic_logo.png" width="400"></a></p>

# Laravel email notification example

## About Teacoders

Tea Coders is an IT consulting and software product development company that designs, develops and deploys solutions based on AI and Machine Learning. These are accessible through web, mobile, and embedded software products for clients across the World. Our customers include start-ups as well as some of the renowned companies. Focused on Artificial Intelligence-driven IoT, we create solutions that address the pressing challenges of the customers

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

// You can use another queue driver if you want and if you don't want to use the queue then don't change it and don't run any commands related to the queue
QUEUE_CONNECTION=database 

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
// open new terminal and run
php artisan queue:work
```

## Credits

- [All Contributors](../../contributors)
