# PHP Bookmark Manager

## Overview
You will design an application that will manage bookmarks for your PHP websites. You will be able to group the bookmarks by Category (I.e Laravel, Symfony, Silex, etc).

## User Management (CRUD)

1. Ability to add, edit, manage (delete), invite Users (CRUD)
2. Ability to add, edit, manage (delete) User Groups (CRUD)

## Bookmarks

1. Ability to add, edit, manage (delete) Bookmarks (CRUD)
2. Ability to add, edit, manage (delete) Bookmark Categories (CRUD)
3. Bonus: Ability to share bookmark with other email addresses
4. Bonus: Ability to attach optional screenshot, just 1
5. Bonus: Make it pretty. Use Bootstrap or Foundation to make it look nice.
6. Bonus: Twitter feed Searching #PHP connecting to twitter API

**SUPER BONUS!!!:** Use codeception to write simple functional test, just watch the videos. It’s not crazy complicated.

## Requirements

  * Laravel 5.1
  * Database MUST use migrations
  * Bonus: Well Documented
  * Tested

## A Laravel-based bookmark manager

## Synopsis 

This is a simple PHP bookmark manager written in Laravel and using Boostrap. Its more a proof-of-concept and not really ready for production... yet.

## Specifications

* Suitable server (LAMP-based)
* A MySQL database for use with Bookmarks (utf8 should be fine)
* Bower (and thus Node/NPM)

## Up and Running
Create your MySQL database and clone this repo into a new vhost/web dir.

Run composer's install option to grab everything for Laravel:
```
composer install
```
Run bower's install option to grab all of the required .js/.css (public/assets/vendor):
```
bower install
```
Copy over .env.example so you have your own preferences file:
```
cp .env.example .env
```
Edit it and modify the last 4 lines:
```
nano .env
```
```
DB_HOST=localhost
DB_DATABASE=bookmarks
DB_USERNAME=user
DB_PASSWORD=password
```
Run Laravel/artisan to generate a new app key:
```
php artisan key:generate
```
Run the migrations and database seeders to get you up and running:
```
php artisan migrate
```
```
php artisan db:seed
```
Set permissions appropriately
```
chmod -R 777 /my/bookmarks/webroot
```
Default user/password is: admin@localhost/password

## Features
* Basic accounts
* Public/private bookmarks
* Filter by visibility & tags
* Search

## Todo
* Tidy up/refactoring
* API
* Favourites
* Profiles
    * Scope settings
    * Themes
    * View settings
* Lots more

## Notes
There is already a .htaccess in the root to rewrite to /public

## License 
The Laravel framework is open-sourced software licensed under the MIT license.
