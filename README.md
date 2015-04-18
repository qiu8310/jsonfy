# jsonfy 
[![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-url]][daviddm-image] [![Coverage Status][coveralls-image]][coveralls-url] [![Code Climate][climate-image]][climate-url]

Parse json like string to json object


## Install

```bash
$ npm install --save jsonfy
```


## Usage

```javascript

var jsonfy = require('jsonfy');
jsonfy('12')                  // result number: 12
jsonfy('"12"')                // result string: '12'
jsonfy('[a, 2.5, true]')      // result array : ['a', 2.5, true] 
jsonfy('{a: a b c, f: 2e2}')  // result object: {a: 'a b c', f: 200}

jsonfy('{str: abc, bool: true, number: 0.24, array: [1,2], emptyObj: {}}');
// return object: {str: 'abc', bool: true, number: 0.24, array: [1, 2], emptyObj: {}}

```

## Feature

* Fully compatible with JSON string
* String can use single quote
* String don't need quote only if it is a number string or it contains characters `]`,`}`,`'` or `"`



## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [gulp](http://gulpjs.com/).


## License

Copyright (c) 2015 Zhonglei Qiu. Licensed under the MIT license.



[climate-url]: https://codeclimate.com/github/qiu8310/jsonfy
[climate-image]: https://codeclimate.com/github/qiu8310/jsonfy/badges/gpa.svg
[npm-url]: https://npmjs.org/package/jsonfy
[npm-image]: https://badge.fury.io/js/jsonfy.svg
[travis-url]: https://travis-ci.org/qiu8310/jsonfy
[travis-image]: https://travis-ci.org/qiu8310/jsonfy.svg?branch=master
[daviddm-url]: https://david-dm.org/qiu8310/jsonfy.svg?theme=shields.io
[daviddm-image]: https://david-dm.org/qiu8310/jsonfy
[coveralls-url]: https://coveralls.io/r/qiu8310/jsonfy
[coveralls-image]: https://coveralls.io/repos/qiu8310/jsonfy/badge.png


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/qiu8310/jsonfy/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

