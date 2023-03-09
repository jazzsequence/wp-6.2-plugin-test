# WordPress 6.2 Tester plugin

Tests some new features of WP 6.2.

## Currently testing

### `move_dir`

An admin page is created with buttons that attempt to use the new `move_dir` command. The assumption is that you are working on an immutable filesystem, so some instances of `move_dir` will be impossible due to file write permissions. The actions will fire regardless and work successfully on systems with full read/write access (e.g. localdev) but the descriptions indicate the expected behavior.

## Uses

* [CMB2/CMB2](https://github.com/CMB2/CMB2) - For an easy-to-bootstrap admin page. Creates a custom field type for the buttons.

## Warnings

This file is not recommended for any kind of production use. There are no nonces and we're moving stuff around the filesystem. Use at your own peril. 😅
