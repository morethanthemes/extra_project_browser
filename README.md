# Extra Project Browser

Project Browser source plugin that exposes recipes prefixed with `extra_` found in your codebase. On install it auto-enables the source in Project Browser settings.

## Installation

- With Composer (Packagist): `composer require morethanthemes/extra_project_browser` (installs to `web/modules/contrib` by default)
- Enable the module: `drush en extra_project_browser -y`

For local development from Git, clone it into your custom modules location and ensure Drupal sees that path (for example with a `web/modules/custom` symlink to your dev directory).

## What it does

- Scans configured recipe locations for `recipe.yml` under directories starting with `extra_`.
- Surfaces those recipes as a Project Browser source (`extra_recipes`).
- Automatically enables the source in `project_browser.admin_settings` on install; removes it on uninstall.

## Development

The module lives in `dev/custom/extra_project_browser`. Keep it under version control separately if you publish to Packagist.
