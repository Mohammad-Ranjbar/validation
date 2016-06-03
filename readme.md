[![Build Status](https://travis-ci.org/anetwork/validation.svg?branch=master)](https://travis-ci.org/anetwork/validation)

# Laravel Persian Validation

Laravel Persian Validation provides validation for Persian alphabet, number and etc.

## Requirement

* Laravel 5.*
* PHP 5.5 >=

## License

Laravel Persian Validation is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

## Install

Via Composer

``` bash
$ composer require Anetwork/Validation
```

##Config

Add the following provider to providers part of config/app.php
``` php
Anetwork\Validation\PersianValidationServiceProvider::class
```

## Usage

You can use it as Validator rules

``` php
Validator::make( $request->all(), [

  'name' => 'persian_alpha',    // validate persian alphabet

  'age' => 'persian_num',   // validate persian numbers

  'address' => 'persian_alpha_num',   // validate persian alphabet & numbers

  'mobile' => 'mobile',   // validate mobile number

  'sheba_number' => 'sheba',    // validate sheba number of bank account

  'melli_code' => 'melliCode',    // validate melli code number

]);
```
