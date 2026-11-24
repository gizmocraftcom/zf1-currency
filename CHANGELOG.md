# Changelog

## 2.0.0

Fork of `diablomedia/zendframework1-currency`, published as `gizmocraft/zendframework1-currency`.

### Breaking changes

- Requires PHP `>=8.5`. Tested on PHP 8.5 and 8.6.
- Package renamed from `diablomedia/zendframework1-currency` to `gizmocraft/zendframework1-currency`. It now requires `gizmocraft/zendframework1-exception`, `-loader`, `-cache` and `-locale`, all `^2.0.0`.

### Other changes

- No public signature changes. `Zend_Currency::__construct()` has an equivalent rewritten condition to satisfy PHPStan; behavior is unchanged.
- Dev dependencies upgraded (PHPUnit 13, PHPStan 2.3, php-cs-fixer 3.95, GrumPHP 2.27). Dropped `composer-require-checker`, which has no release for PHP 8.6.
- Tests migrated to PHPUnit 13 attributes. CI runs PHP 8.5 and 8.6.
