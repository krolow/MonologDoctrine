# DoctrineMonolog

Doctrine Monolog, makes monolog meets Doctrine as a SQL Logger


### Usage

```php
	$paths = array(
    		'entityFolder',
	);
	$config = Setup::createAnnotationMetadataConfiguration($paths, true);
	$config->setSQLLogger(new MonologSQLLogger(null, null, __DIR__ . '/path/of/log/'));
```

By default the first two params can be null, or you can pass one instance of Monolog\Logger and Monolog\Handler\StreamHandler and the third param won't be necessary in this case.

### License


