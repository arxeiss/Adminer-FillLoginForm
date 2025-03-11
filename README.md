# Adminer-FillLoginForm

[![Adminer](https://img.shields.io/badge/adminer-%3E%3D5.0-blue)](https://www.adminer.org)

Adminer plugin for filling login form by set values

- How to install plugins to Adminer: http://www.adminer.org/plugins/
- About plugin on http://www.kutac.cz/blog/weby-a-vse-okolo/adminer-plugin-fill-login-form/ (🇨🇿 - Czech only)

## Usage

> :warning: In production this can reveal your credentials, use carefully! :warning:

```php
$plugins = [
    /*
      Params
      1. DB type - "server" == MySQL, others are sqlite, sqlite2, pgsql, oracle, mssql, firebird, simpledb, mongo, elastic
      2. server - localhost by default
      3. login
      4. password
      5. DB name
    */
    new FillLoginForm("server","","root","","")
];
```

## Changelog

## v2.0

- Add support for Adminer 5

## v1.1

- Fix JS according to CSP (Content Security Policy). Added in Adminer [4.4.0 (released 2018-01-17)](https://github.com/vrana/adminer/blob/master/changes.txt)

## v1.0
Initial release
