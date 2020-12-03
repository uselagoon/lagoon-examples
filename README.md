# Lagoon Examples

All of these examples are collected here to enable discovery, testing and cross-referencing


## Adding a new example

The folders are added as submodules from the branches of the host projects
To add a new example:

1. `git submodule add -b 9.x-php8 https://github.com/amazeeio/drupal-example-simple.git drupal9-php8`
2. `git submodule update --init`

To refresh local submodules
1. `git submodule update --remote`

## Testing examples

This repository uses [Leia](https://github.com/lando/leia) from the awesome Lando team to run tests.

There are a selection of tests defined in the source repos.

To generate and run tests you need yarn installed:

1. `yarn install`
2. `yarn generate-tests`
3. Look at the scripts section in package.json to select which tests to run.
4. e.g. `yarn test:all` will run all tests

