[![Build Status](https://travis-ci.org/ORNAJS/orna-npm-base.svg?branch=master)](https://travis-ci.org/ORNAJS/orna-npm-base) [![npm version](https://badge.fury.io/js/orna-npm-base.svg)](http://badge.fury.io/js/orna-npm-base) [![Dependency Status](https://david-dm.org/ORNAJS/orna-npm-base.svg)](https://david-dm.org/ORNAJS/orna-npm-base) [![devDependency Status](https://david-dm.org/ORNAJS/orna-npm-base/dev-status.svg)](https://david-dm.org/ORNAJS/orna-npm-base#info=devDependencies) 
# orna-npm-base

A base package for creating NPM packages with ES2015.

Writing in ES2015 is an amazing experience. Setting up babel and the development environment in a kind of a pain.

If you want to write a **NPM module** in ES2015 and publish to NPM with backward compatibility, this is the **easiest** way.

---
## Stats

[![npm downloads](https://img.shields.io/npm/dm/norna-npm-base.svg)](https://npmjs.org/orna-npm-base)

[![Throughput Graph](https://graphs.waffle.io/ORNAJS/orna-npm-base/throughput.svg)](https://waffle.io/ORNAJS/orna-npm-base/metrics)

## Basic Usage

* Simply clone [this](https://github.com/ORNAJS/orna-npm-base) project.
* `git clone git@github.com:/ORNAJS/orna-npm-base <Project Name>`
* Change the `package.json` as you want.
* `lib/index.js` in your entry point.
* Then publish to npm via `npm publish`.

## Linting

* ESLINT support is added to the project.
* It's configured for ES2015
* Use `npm run lint` to lint your code and `npm run lintfix` to fix common issues.

## Testing

* You can write test under `__test__` directory anywhere inside `lib` including sub-directories.
* Then run `npm test` to test your code. (It'll lint your code as well).
* You can also run `npm run testonly` to run tests without linting.

## ES2015 Setup

* ES2015 support is added with babel6.
* After you publish your project to NPM, it can be run on older node versions and browsers without the support of Babel.
* This project uses ES2015 and some of the upcoming features like `async await`.
* You can change them with adding and removing [presets](http://jamesknelson.com/the-six-things-you-need-to-know-about-babel-6/).
* All the polyfills you use are taken from the local `babel-runtime` package. So, this package won't add any global polyfills and pollute the global namespace.

