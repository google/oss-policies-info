# Foundational PHP Support

The relevant policies are described at
https://cloud.google.com/php/getting-started/supported-php-versions. This
document captures the specific version numbers as resolved by those policies.

### Cited Text

> The Cloud Client Libraries for PHP are compatible with at least the three most
> recent, major PHP releases. The libraries will always be compatible with at
> least one GA runtime for App Engine and Cloud Run functions.

PHP runtime documentation from Cloud Run: https://docs.cloud.google.com/run/docs/runtimes/php
PHP runtime documentation from App Engine: https://docs.cloud.google.com/appengine/docs/flexible/php/runtime

Generally speaking, Composer configuration should be automatic.

### Implied Support Matrix

| Dimension   | Supported Version | Last Changed | Next Change [^next-change] |
|-------------|-------------------|--------------|----------------------------|
| PHP Version | >= 8.2            | 2024-12-17   | 2026-12-31                 |
| Composer    | >= 2.10           | 2026-09-17   | 2026-12-31                 |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

