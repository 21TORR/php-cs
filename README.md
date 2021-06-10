Code Style for PHP
==================

Installation
------------

You should install this package using the [composer-bin-plugin]. So first add the composer plugin, then install this bundle:

```bash
composer req --dev bamarni/composer-bin-plugin
composer bin test require --dev 21torr/php-cs
composer bin cs-fixer require --dev friendsofphp/php-cs-fixer
```

Afterwards add the following scripts to your `composer.json`, to always and automatically keep these dependencies up to date:

```json
"scripts": {
    "post-install-cmd": [
        "@composer bin all install --ansi"
    ],
    "post-update-cmd": [
        "@composer bin all update --ansi"
    ]
}
```

Usage
-----

After installation, you can run the tools like this:

```bash
./vendor/bin/php-cs-fixer fix --dry-run --diff --config vendor-bin/test/vendor/21torr/php-cs/.php_cs.dist
./vendor/bin/phpstan analyze -c vendor-bin/test/vendor/21torr/php-cs/phpstan/lib.neon .
```

In a project (instead of a lib) you should use

```bash
./vendor/bin/phpstan analyze -c vendor-bin/test/vendor/21torr/php-cs/phpstan/symfony.neon .
```

For [composer normalize], you can just install the plugin globally and run it.


Editor Config
-------------

This library also includes the default `.editorconfig`. Just symlink this file to your project root.


[composer-bin-plugin]: https://github.com/bamarni/composer-bin-plugin
[composer normalize]: https://packagist.org/packages/ergebnis/composer-normalize
