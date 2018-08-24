# Install WordPress test environment

It installs WordPress test environment for PHPUnit.

## How to use

Run following command.

```
$ curl -L https://raw.githubusercontent.com/naogify/install-wp-test-env/master/install.sh | bash
```

If you have DB informations, add `-s` option. 

```
$ curl -L https://raw.githubusercontent.com/naogify/install-wp-test-env/master/install.sh | bash -s <db-name> <db-user> <db-pass> [db-host] [wp-version]
```

Then, this script will downlod `test-template.php` to `tests/test-template.php`. This is the template file for unit test. Please edit it.

## Requires

* PHPUnit
* WP-CLI

## Running PHPUnit

```
$ wp scaffold plugin <plugin-slug>
$ cd <plugin-slug>
$ phpunit
```
