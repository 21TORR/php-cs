4.1.0
=====

* (improvement) Bump dependencies.
* (improvement) Require PHP 8.2+.


4.0.4
=====

*	(improvement) Don't use deprecated PHPStan config.


4.0.3
=====

*	(improvement) Bump dependencies.


4.0.2
=====

*	(improvement) Don't use overly strict rules.


4.0.1
=====

*	(bug) Fix accidentally activated rules


4.0.0
=====

*	(bc) Bump to PHP-CS-Fixer v3.
*	(improvement) Bump required minimum PHP version to 8.0


3.0.1
=====

*	(improvement) Fix deprecations in PHP-CS-Fixer
*	(improvement) Keep using the `test` vendor bin directory for the main installation


3.0.0
=====

*	(feature) Update packages + add `phpstan-strict-rules` and `phpstan-deprecation-rules` extensions.
*	(bc) PHP-CS-Fixer must now be installed separately.
*	(internal) Validate PHP-CS-Fixer config in CI.


2.0.9
=====

*   (improvement) Directly include `composer-normalize` in this package.


2.0.8
=====

*   (improvement) Add "custom" as directory for PHP-CS-Fixer.


2.0.7
=====

*   (improvement) Allow PHP 7.2


2.0.6
=====

*   (improvement) Allow PHP 8.0


2.0.5
=====

*   (improvement) Disable `checkGenericClassInNonGenericObjectType:` in PhpStan.


2.0.4
=====

*   (improvement) Disable `checkMissingIterableValueType` in PhpStan.


2.0.3
=====

*   (improvement) Don't force blank line before `yield`.


2.0.2
=====

*   (improvement) Also run PHP CS Fixer in the `tests/` directory.


2.0.1
=====

*   (improvement) Use tabs for indentation.


2.0.0
=====

*   (bc) Use PhpStan instead of Psalm.


1.0.2
=====

*   (improvement) Ignore `UnusedClass` for libraries.


1.0.1
=====

*   (improvement) Separate configs for libs + projects.


1.0.0
=====

Initial implementation `\o/`
