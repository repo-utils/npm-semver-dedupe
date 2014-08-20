
# npm-semver-dedupe

[![NPM version][npm-image]][npm-url]
[![Dependency Status][david-image]][david-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]
[![Gittip][gittip-image]][gittip-url]

Here's a crazy idea: remove all semver-compatible duplicates!
If your top-level module uses `module@1.1.2` and a dependency
uses `module@1.0.0`, `npm-semver-dedupe` will simply remove `module@1.0.0`,
even if it explicitly wants `v1.0.0`.

Yes, this might break your app. Yes, this is very hacky.
However, duplicates suck and so does `npm dedupe`.
You don't need 20 copies of the same version of esprima in your app.

__If you run this, you better test your app afterwards because something is very likely to break!__

## Usage

```
npm i -g npm-semver-dedupe
npm-semver-dedupe
```

This will dedupe the current app/module.

[npm-image]: https://img.shields.io/npm/v/npm-semver-dedupe.svg?style=flat-square
[npm-url]: https://npmjs.org/package/npm-semver-dedupe
[github-tag]: http://img.shields.io/github/tag/repo-utils/npm-semver-dedupe.svg?style=flat-square
[github-url]: https://github.com/repo-utils/npm-semver-dedupe/tags
[travis-image]: https://img.shields.io/travis/repo-utils/npm-semver-dedupe.svg?style=flat-square
[travis-url]: https://travis-ci.org/repo-utils/npm-semver-dedupe
[coveralls-image]: https://img.shields.io/coveralls/repo-utils/npm-semver-dedupe.svg?style=flat-square
[coveralls-url]: https://coveralls.io/r/repo-utils/npm-semver-dedupe?branch=master
[david-image]: http://img.shields.io/david/repo-utils/npm-semver-dedupe.svg?style=flat-square
[david-url]: https://david-dm.org/repo-utils/npm-semver-dedupe
[license-image]: http://img.shields.io/npm/l/npm-semver-dedupe.svg?style=flat-square
[license-url]: LICENSE.md
[downloads-image]: http://img.shields.io/npm/dm/npm-semver-dedupe.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/npm-semver-dedupe
[gittip-image]: https://img.shields.io/gittip/jonathanong.svg?style=flat-square
[gittip-url]: https://www.gittip.com/jonathanong/
