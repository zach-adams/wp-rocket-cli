## CLI interface for the WP Rocket

This repository contains a [WP-CLI command](https://github.com/wp-cli/wp-cli)  for the [WP Rocket](http://wp-rocket.me) plugin. After installing this plugin, you will have access to a `wp rocket` command.

Currently supported commands:

* `wp rocket activate` -- Set WP_CACHE to true.
* `wp rocket deactivate` -- Set WP_CACHE to false.
* `wp rocket clean --post_id=<post_id> --permalink=<permalink> --lang=<lang> --blog_id=<blog_id> --confirm` -- Purge cache files.
* `wp rocket preload` -- Preload cache files.
* `wp rocket regenerate --file=<file>` -- Regenerate .htaccess, advanced-cache.php or the WP Rocket config file.
    
## Installing

If you're using WP-CLI v0.23.0 or later, you can install this package with:

```
wp package install zach-adams/wp-rocket-cli
```

## Changelog

### 1.2

* Add `--confirm` flag for `clean` command so it can be confirmed automatically.

### 1.1

* Add `regenerate` command.

### 1.0

* Initial release
