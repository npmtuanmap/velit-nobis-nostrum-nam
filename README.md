# @npmtuanmap/velit-nobis-nostrum-nam <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Set? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isSet = require('@npmtuanmap/velit-nobis-nostrum-nam');
assert(!isSet(function () {}));
assert(!isSet(null));
assert(!isSet(function* () { yield 42; return Infinity; });
assert(!isSet(Symbol('foo')));
assert(!isSet(1n));
assert(!isSet(Object(1n)));

assert(!isSet(new Map()));
assert(!isSet(new WeakSet()));
assert(!isSet(new WeakMap()));

assert(isSet(new Set()));

class MySet extends Set {}
assert(isSet(new MySet()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@npmtuanmap/velit-nobis-nostrum-nam
[npm-version-svg]: https://versionbadg.es/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam.svg
[deps-svg]: https://david-dm.org/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam.svg
[deps-url]: https://david-dm.org/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam
[dev-deps-svg]: https://david-dm.org/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@npmtuanmap/velit-nobis-nostrum-nam.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@npmtuanmap/velit-nobis-nostrum-nam.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@npmtuanmap/velit-nobis-nostrum-nam.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@npmtuanmap/velit-nobis-nostrum-nam
[codecov-image]: https://codecov.io/gh/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@npmtuanmap/velit-nobis-nostrum-nam
[actions-url]: https://github.com/npmtuanmap/velit-nobis-nostrum-nam/actions
