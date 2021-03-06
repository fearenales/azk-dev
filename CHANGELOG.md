# Change Log

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## dev

* Enhancements
  * [Core] Updating `dotenv`;

## v0.3.0 - (2016-01-12)

* Deprecations
  * [Specs] `--slow` is not supported, all tests are performed by standard now. The `--skip-slow` option comes into existence as inverse replacement;

## v0.2.1 - (2016-01-05)

* Deprecations
  * [jscs] `validateJSDoc` is deprecated, use `jsDoc` in replace;
  * [Core] Adding dependencie `jshint` and turning `babel-polyfill` a optional dependencie;
  * [gulp] Replacing `gulp-clean` and `rimraf` for `del` and `vinyl-paths`;

## v0.2.0 - (2016-01-04)

* Enhancements
  * [Core] Modularizing `AzkGulp` in more pieces;
  * [Generators] Adding support to use generators and promises in tests;
  * [Chai] Adding chai-subset and change load order of the chai plugins;
  * [Babel] Adding `babel:polyfill:install` gulp task, to assist in the installation of the `babel-polyfill` lib;
  * [Babel] Adding `babel:core:version` gulp task, it helps to find out the version of the babel `azk-dev` this using;
  * [Babel] Configure babel for use present `es2015` and plugin `add-module-exports` by default;
  * [Sourcemap] Refactoring sourcemap to use a format `[module]-[version] [relative_path]`

* Deprecations
  * [Babel] The "runtime" option is no longer default, and its use generates a depreciation alert. The dependence "babel-polyfill" should be used instead;
  * [Require] The loading of files from the root directory become discouraged, files should be loaded from the lib folder, as the example: `require('azk-dev/chai') => require('azk-dev/lib/chai')`;
