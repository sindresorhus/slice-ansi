# slice-ansi [![Build Status](https://travis-ci.org/chalk/slice-ansi.svg?branch=master)](https://travis-ci.org/chalk/slice-ansi)

> Slice a string with [ANSI escape codes](http://en.wikipedia.org/wiki/ANSI_escape_code#Colors_and_Styles)


## Install

```
$ npm install --save slice-ansi
```


## Usage

```js
var chalk = require('chalk');
var sliceAnsi = require('slice-ansi');

var input = 'The quick brown ' + chalk.red('fox jumped over ') +
	'the lazy ' + chalk.green('dog and then ran away with the unicorn.');

console.log(sliceAnsi(input, 20, 30));
```

## API

### sliceAnsi(input, columns)

#### input

Type: `string`

String with ANSI escape codes. Like one styled by [`chalk`](https://github.com/chalk/chalk).

#### beginSlice

Type: `number`

The zero-based index at which to begin the slice.

#### endSlice

Type: `number`

Optional. The zero-based index at which to end the slice.


## Related

- [chalk](https://github.com/chalk/chalk) - Terminal string styling done right


## License

MIT © [David Caccavella](https://githbu.com/dthree)
