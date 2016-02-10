angular-gettext-cli [![Build Status](https://travis-ci.org/huston007/angular-gettext-cli.svg?branch=master)](https://travis-ci.org/huston007/angular-gettext-cli)
===================

A command line interface for [angular-gettext-tools](https://github.com/rubenv/angular-gettext-tools)

## Installation

`npm install angular-gettext-cli -g` for global using or
`npm install angular-gettext-cli --save-dev` for local.

## Extraction:

`angular-gettext-cli  --files "./app/*.+(js|html)" --dest ./extract.pot --marker-name i18n`

### Parameters:
* `--files` - a [glob](https://github.com/isaacs/node-glob) pattern to specify files to process
* `--dest` - path to file to write extracted words.
* `--marker-name` - a name of marker to search in js-files (see [angular-gettext-tools](https://github.com/rubenv/angular-gettext-tools#options))

## Compilation:

`angular-gettext-cli  --compile --files 'test/*.po' --dest test/output.js --format javascript --module gettext-test`

### Parameters:
* `--files` - a [glob](https://github.com/isaacs/node-glob) pattern to specify files to process
* `--dest` - path to file to write extracted words.
* `--format` - `javascript` or `json`
* `--module` - For the `javascript` output format, the angular module name to use in the output file.

For more options, see [angular-gettext-tools](https://github.com/rubenv/angular-gettext-tools#options).
