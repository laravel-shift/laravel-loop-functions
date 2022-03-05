![Laravel Loop Functions](https://user-images.githubusercontent.com/37669560/154233514-72078240-d8c5-4b71-acc0-9e3afe5e52e2.png)

# Laravel Loop Functions
[![Latest Version on Packagist](https://img.shields.io/packagist/v/michael-rubel/laravel-loop-functions.svg?style=flat-square&logo=packagist)](https://packagist.org/packages/michael-rubel/laravel-loop-functions)
[![Total Downloads](https://img.shields.io/packagist/dt/michael-rubel/laravel-loop-functions.svg?style=flat-square&logo=packagist)](https://packagist.org/packages/michael-rubel/laravel-loop-functions)
[![Code Quality](https://img.shields.io/scrutinizer/quality/g/michael-rubel/laravel-loop-functions.svg?style=flat-square&logo=scrutinizer)](https://scrutinizer-ci.com/g/michael-rubel/laravel-loop-functions/?branch=main)
[![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/michael-rubel/laravel-loop-functions.svg?style=flat-square&logo=scrutinizer)](https://scrutinizer-ci.com/g/michael-rubel/laravel-loop-functions/?branch=main)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/michael-rubel/laravel-loop-functions/run-tests/main?style=flat-square&label=tests&logo=github)](https://github.com/michael-rubel/laravel-loop-functions/actions)
[![PHPStan](https://img.shields.io/github/workflow/status/michael-rubel/laravel-loop-functions/phpstan/main?style=flat-square&label=larastan&logo=laravel)](https://github.com/michael-rubel/laravel-loop-functions/actions)

The package provides the collection of methods to loop over your data.

The package requires PHP `^8.x` and Laravel `^8.71` or `^9.0`.

## Installation
Install the package using composer:
```bash
composer require michael-rubel/laravel-loop-functions
```

## Usage
```php
use LoopFunctions;
```

## Available methods
Assign Eloquent model attributes to class properties:
```php
$this->attributesToProperties($model);
```

Assign array key values to class properties:
```php
$this->arrayToProperties($data);
```

## Logging
As the package doesn't throw an error in case of failed assignment (for example type incompatibility), you may wish to log such an event. The package has failed assignment logging disabled by default, but you can turn it on by publishing the config:

```bash
php artisan vendor:publish --tag="loop-functions-config"
```

## Testing
```bash
composer test
```
