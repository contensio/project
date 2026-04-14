# Contensio — Laravel Project Scaffold

A pre-configured Laravel 13 application ready to run [Contensio CMS](https://github.com/contensio/contensio).

> 🚧 **Work in progress** — this scaffold will become installable via Composer once `contensio/contensio` is published to Packagist. Watch the repo to be notified when v1.0 ships.

## Planned install

```bash
composer create-project contensio/project my-site
cd my-site
php artisan contensio:install
```

## What's inside

This repo is a standard Laravel 13 application with Contensio CMS pre-required and the default theme placed under `packages/themes/contensio/default/`.

When installed, it includes:

- Laravel 13 application skeleton
- [`contensio/contensio`](https://github.com/contensio/contensio) as a dependency
- `packages/themes/` — ready-to-activate default theme, room for additional themes
- `packages/plugins/` — ready for plugin installations

## Requirements

- PHP 8.3+
- Composer 2.x
- MySQL 8 / PostgreSQL 14 / SQLite 3
- Node 20+ (for asset pipeline)

## Development

If you're developing Contensio itself and want to run this scaffold against a local checkout of the core package, add a path repository in your local `composer.json` (not committed):

```json
"repositories": [
    { "type": "path", "url": "../contensio" }
]
```

Then run `composer update contensio/contensio`.

## License

Copyright © 2026 Iosif Gabriel Chimilevschi. Licensed under [AGPL-3.0-or-later](https://www.gnu.org/licenses/agpl-3.0.txt).
