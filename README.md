yii-airbrake
============
An integration of <a href="https://github.com/dbtlr/php-airbrake" target="_blank">php-airbrake</a> to drop into Yii in place of CErrorHandler.

## Installation ##

Add the following to the `require` object in your `composer.json`:

```json
  "require": {
    ...
    "markokeeffe/yii-airbrake": "dev-master"
  },
```

Update composer:

```bash
$ composer update
```

Add the ErrorHandler application component into the Yii 'errorHandler' component in your config:

```php
  'errorHandler'=>array(
    'class'=>'ErrorHandler',
    'apiKey' => '...',
    'endpoint'=>'http://example.com',
    'environment'=>'Testing',
  ),
```
