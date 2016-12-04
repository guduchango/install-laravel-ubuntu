# Install laravel on ubuntu

### Install mysql server
```
sudo apt-get install mysql-server
```
### Install some necesary libraries
```
sudo apt-get install php7.0 libapache2-mod-php7.0 php7.0-mbstring php7.0-zip php7.0-xml php7.0-mysql curl php7.0-cli php7.0-soap
```
### Install composer
```
curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer
```
### Change options php.ini
```
gedit /etc/php/7.0/cli/php.ini 

## Change this options
display_errors = On
upload_max_filesize = 50M
```
### Run laravel
```
php artisan serve
```
## Miscellaneous
```
### into de proyect
$ composer install
$ composer dump-auto
$ php artisan key:generate
$ php artisan clear-copiled
$ php artisan route:list

### copy .env file
cp ./.env.example ./.env

### change .env database config
DB_CONNECTION=mysql
DB_HOST=localhost
DB_DATABASE=foo
DB_USERNAME=foo
DB_PASSWORD=secret
```

