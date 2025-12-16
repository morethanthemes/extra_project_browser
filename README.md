# Extra Project Browser

Project Browser source plugin that exposes recipes prefixed with `extra_` found in your codebase. On install it auto-enables the source in Project Browser settings.

## Installation

- With Composer: `composer require morethanthemes/extra_project_browser`
- Enable the module: `drush en extra_project_browser -y`

If your codebase keeps custom modules outside the docroot, ensure `web/modules/custom` is linked to your custom modules directory.

## What it does

- Scans configured recipe locations for `recipe.yml` under directories starting with `extra_`.
- Surfaces those recipes as a Project Browser source (`extra_recipes`).
- Automatically enables the source in `project_browser.admin_settings` on install; removes it on uninstall.

## Development

The module lives in `dev/custom/extra_project_browser`. Keep it under version control separately if you publish to Packagist.
