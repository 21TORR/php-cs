Code Style for PHP
==================

Installation
------------

You should install this package using the [composer-bin-plugin]:

```bash
composer bin test require --dev 21torr/php-cs
```

Usage
-----

After installation, you can run the tools like this:

```bash
./vendor/bin/php-cs-fixer fix --dry-run --diff --config vendor-bin/test/vendor/21torr/php-cs/.php_cs.dist
./vendor/bin/psalm --threads=8 -c vendor-bin/test/vendor/21torr/php-cs/psalm.xml
```

For [composer normalize], you can just install the plugin globally and run it.


[composer-bin-plugin]: https://github.com/bamarni/composer-bin-plugin
[composer normalize]: https://packagist.org/packages/ergebnis/composer-normalize