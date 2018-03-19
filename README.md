# nanoseconds [![NPM version](https://img.shields.io/npm/v/nanoseconds.svg?style=flat)](https://www.npmjs.com/package/nanoseconds) [![NPM monthly downloads](https://img.shields.io/npm/dm/nanoseconds.svg?style=flat)](https://npmjs.org/package/nanoseconds) [![NPM total downloads](https://img.shields.io/npm/dt/nanoseconds.svg?style=flat)](https://npmjs.org/package/nanoseconds) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/nanoseconds.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/nanoseconds)

> Convert the process.hrtime() array to a single nanoseconds value. This makes it easier to diff times.

Please consider following this project's author, [Jon Schlinkert](https://github.com/jonschlinkert), and consider starring the project to show your :heart: and support.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save nanoseconds
```

## Usage

```js
const nano = require('nanoseconds');
console.log(nano(process.hrtime()));
//=> 725220674029406
```

**Examples**

```js
nano([0, 999]);
//=> 999

nano([12, 999]);
//=> 12000000999

nano(['1298001', '09187662']);
//=> 1298001009187662
```

## About

<details>
<summary><strong>Contributing</strong></summary>

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

</details>

<details>
<summary><strong>Running Tests</strong></summary>

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

</details>

<details>
<summary><strong>Building docs</strong></summary>

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

</details>

### Related projects

You might also be interested in these projects:

* [o-clock](https://www.npmjs.com/package/o-clock): Simple javascript utility for displaying the time in 12-hour clock format. | [homepage](https://github.com/jonschlinkert/o-clock "Simple javascript utility for displaying the time in 12-hour clock format.")
* [pretty-time](https://www.npmjs.com/package/pretty-time): Easily format the time from node.js `process.hrtime`. Works with timescales ranging from weeks to nanoseconds. | [homepage](https://github.com/jonschlinkert/pretty-time "Easily format the time from node.js `process.hrtime`. Works with timescales ranging from weeks to nanoseconds.")
* [time-stamp](https://www.npmjs.com/package/time-stamp): Get a formatted timestamp. | [homepage](https://github.com/jonschlinkert/time-stamp "Get a formatted timestamp.")
* [timescale](https://www.npmjs.com/package/timescale): Convert from one time scale to another. Nanosecond is the most atomic unit, week is… [more](https://github.com/jonschlinkert/timescale) | [homepage](https://github.com/jonschlinkert/timescale "Convert from one time scale to another. Nanosecond is the most atomic unit, week is the largest unit.")

### Author

**Jon Schlinkert**

* [LinkedIn Profile](https://linkedin.com/in/jonschlinkert)
* [GitHub Profile](https://github.com/jonschlinkert)
* [Twitter Profile](https://twitter.com/jonschlinkert)

### License

Copyright © 2018, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on March 19, 2018._