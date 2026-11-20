# Meatpress Helpers

Meatpress Helpers provides a single `__()` translation function for Laravel and WordPress. [Meatpress Framework](https://github.com/digitalmeat/meatpress-framework) installs it as a Composer dependency. The package loads before Laravel's helpers and works with the WordPress core patch included in [the Framework repository](https://github.com/digitalmeat/meatpress-framework/blob/main/patches/wordpress-core.patch).

## Usage

```php
__('Read more', 'meat-theme');
__('orders.shipping', ['brand' => 'MEAT']);
__('Read more');
```

A string in the second argument selects a WordPress text domain. With an array or an omitted second argument, the helper looks for a Laravel string translation first, then falls back to WordPress's default domain. Named replacements are also applied on fallback.

## Contributing

```bash
composer install
composer test
composer test:lint
```

## Security vulnerabilities

Report suspected vulnerabilities privately to the MEAT Code maintainers.

## License

Meatpress Helpers is licensed under the [MIT License](LICENSE).
