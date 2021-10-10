<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Setup

 1. Clone the project
 2. Change in the project folder
 3. Run `composer install`
 4. Copy the `.env.example` to `.env`
 5. Setup the your database in the `.env` file
 6. Add these lines at the end of the `.env` file  
```
LDAP_LOGGING=true
LDAP_CONNECTION=default
LDAP_HOST=dc-control
LDAP_USERNAME="admin_login"
LDAP_PASSWORD="admin_password"
LDAP_PORT=389
LDAP_BASE_DN="dc=dc,dc=local"
LDAP_TIMEOUT=5
LDAP_SSL=false
LDAP_TLS=false
```
 7. Run `php artisan key:generate`
 8. Run `php artisan migrate`
 9. Open site and login with username `einstein` and password `password` (Check [Online LDAP Test Server](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/) for more information of the Online LDAP Test Server)
