# Meatpress Helpers

A single `__()` for Laravel and WordPress in a Meatpress application: Laravel keys (`__('auth.failed')`, replacements) go to Laravel's translator, WordPress strings and text domains (`__('Read more', 'my-theme')`) to WordPress's.

It is a separate package from [`digitalmeat/meatpress-framework`](https://github.com/digitalmeat/meatpress-framework) on purpose: its `helpers.php` must be autoloaded **before** Laravel's, which declares `__()` too, so this package depends on nothing but PHP. The framework requires it.

```bash
composer test   # Pest
```

MIT — see [LICENSE](LICENSE).
