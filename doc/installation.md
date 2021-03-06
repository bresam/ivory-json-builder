# Installation

To install the Ivory JSON builder library, you will need [Composer](http://getcomposer.org). It's a PHP 5.3+ dependency
manager which allows you to declare the dependent libraries your project needs and it will install & autoload them for
you.

## Set up Composer

Composer comes with a simple phar file. To easily access it from anywhere on your system, you can execute:

```
$ curl -s https://getcomposer.org/installer | php
$ sudo mv composer.phar /usr/local/bin/composer
```

## Install dependencies

Require the library in your `composer.json` file:

``` bash
$ composer require ivory/json-builder
```

Composer will automatically download your dependencies & create an autoload file in the ``vendor`` directory.

## Autoload

So easy, you just have to require the generated autoload file and you are already ready to play:

``` php
<?php

require __DIR__.'/vendor/autoload.php';

use Ivory\JsonBuilder;

// ...
```

The Ivory JSON Builder library follows the [PSR-4 Standard](http://www.php-fig.org/psr/psr-4/). If you prefer install
it manually, it can be autoload by any convenient autoloader.
