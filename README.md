# bucketcode
This is a Laravel User profile app, Login/Register, Create, Delete Update User details also can create blog, post and delete, Resettig password also

# To Install app
- clone

cd in to directory and run the following dependences

- composer install

Note after composer install if you encounter any error, goto 

vendor/laravel/framework/src/Illuminate/Foundation/PackageManifest.php

and comment the line below

$packages = json_decode($this->files->get($path), true);

then add this 2 lines of codes

$installed = json_decode($this->files->get($path), true);

$packages = $installed['packages'] ?? $installed;

- the run (composer install) again

- create a copy of the .env file

copy .env.example .env

create an empty DB in either Xampp or Wamp (i.e DB_Name bucketcodes with utf8-general_ci)
then change the respective details in you new .env file

- php artisan key:generate

- php artisan db:seed

- php artisn serve

#and that powers up ur site....enter the url and enjoy
