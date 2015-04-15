# Loadsys CakePHP Plugin Skeleton

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)

Basic Skeleton for developing and creation of Loadsys CakePHP Plugins

## Instructions

* Move the `LICENSE_TEMPLATE.md` to your new plugin repo as `LICENSE.md`
* Move the `README_TEMPLATE.md` to your new plugin repo as `README.md`
* Move the `.travis_template.yml` to your new plugin repo as `.travis.yml`
* Move the `.composer_template.json` to your new plugin repo as `.composer.json`

* Edit each of the above files
* The majority of the changes are the `{PLUGIN_SHORT_NAME}` and `{PLUGIN_NAME}` and `{PLUGIN_COMPOSER_NAME}` tags to be replaced
* `{PLUGIN_NAME}` is the name of the repo on GitHub, ie. this plugin is `CakePHP-Plugin-Skeleton`
* `{PLUGIN_SHORT_NAME}` is the name of the plugin as installed in CakePHP, ie. this plugin would be `Skeleton`
* `{PLUGIN_COMPOSER_NAME}` is the name of the plugin as availble through Composer and Packagist, ie this plugin would be `cakephp-plugin-skeleton`
* The Composer name once published on Packagist can not be changed, so ensure you get this right the first time.
* The Loadsys Standard is to use the name of the repo in lower case and dashes to separate words, ie: `loadsys/cakephp-something-words-here`
* Refer to the [Packagist about page](https://packagist.org/about) for more information on Packagist naming conventions
* Finish filling out the `README.md`
* To add the plugin to Travis:
 * note a user with GitHub admin credetionals for the plugin must do this step
 * Visit: https://travis-ci.org/repositories
 * Add the plugin
 * Set the settings for the Plugin to only build when a `.travis.yml` file is present

* To add the plugin to Coveralls for Code Coverage Reports:
 * Any user with merely read access to the GitHub repo can do this
 * Visit: https://coveralls.io/
 * Add the plugin, via the "Add Repos" button
 * Set the settings for the Plugin to:
 * NO: Leave Comments
 * YES: Use Status API
 * Coverage Threshold for Failure: internal recommendation is 70% but you can and should set it higher as you add code coverage
 * Coverage Decrease Threshold for Failure: internal recommendation is 5% but you can set it lower as you add code coverage

* To add the plugin to Packagist for use with Composer:
 * Portions of this can be done by any user, some steps require a GitHub admin
 * Visit: https://packagist.org/
 * Click the "Submit Package" button
 * Fill out the details of the plugin
 * Have a GitHub admin ensure the Callback is set so Packagist will be auto-updated with new versions and branches
 * Recommendation is to have at least two people listed as maintainers on every plugin published via Packagist

* Create a GitHub Token
 * Create a GitHub Token that has only read/write access to your public repos
 * Visit: https://github.com/settings/tokens/new
 * Create a token with only the `public_repo` checked, please ensure only this scope is checked
 * Copy the token
 * Navigate via the command line to the git repo for your Plugin's code 
 * Encrypt the token using the CLI: `travis encrypt 'GITHUB_TOKEN={TOKEN_FROM_GITHUB}'`
 * Note if you wish to not use a Github token you can, however we have issues with Travis hitting GitHub's public API limits, the provided `.travis.yml` will need to be changed to support this however.
 * The Github token is encrypted and only stored/published in it's encrypted format, you can explore the [Travis docs for more information into the encrypt CLI](http://docs.travis-ci.com/user/encryption-keys/) if you have more questions.

## Contributing

### Reporting Issues

Please use [GitHub Isuses](https://github.com/loadsys/CakePHP-Plugin-Skeleton/issues) for listing any known defects or issues.

### Development

When developing this plugin, please fork and issue a PR for any new development.

## License ##

[MIT](https://github.com/loadsys/CakePHP-Plugin-Skeleton/blob/master/LICENSE.md)


## Copyright ##

[Loadsys Web Strategies](http://www.loadsys.com) 2015
