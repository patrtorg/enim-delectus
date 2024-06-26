# @patrtorg/enim-delectus [![ci][ci-image]][ci-url] [![npm][npm-image]][npm-url] [![downloads][downloads-image]][downloads-url] [![javascript style guide][standard-image]][standard-url]

[ci-image]: https://img.shields.io/github/workflow/status/feross/@patrtorg/enim-delectus/ci/master
[ci-url]: https://github.com/patrtorg/enim-delectus/actions
[npm-image]: https://img.shields.io/npm/v/@patrtorg/enim-delectus.svg
[npm-url]: https://npmjs.org/package/@patrtorg/enim-delectus
[downloads-image]: https://img.shields.io/npm/dm/@patrtorg/enim-delectus.svg
[downloads-url]: https://npmjs.org/package/@patrtorg/enim-delectus
[standard-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[standard-url]: https://standardjs.com

### Cross-platform .zip file creation

## install

```
npm install @patrtorg/enim-delectus
```

## usage

```js
var zip = require('@patrtorg/enim-delectus')

var inPath = path.join(__dirname, 'myFolder') // folder to zip
var outPath = path.join(__dirname, 'myFile.zip') // name of output zip file

zip.zipSync(inPath, outPath)
```

## api

### `zip.zip(inPath, outPath, [callback])`

Zip the folder at `inPath` and save it to a .zip file at `outPath`. If a `callback`
is passed, then it is called with an `Error` or `null`.

### `zip.zipSync(inPath, outPath)`

Sync version of `zip.zip`.

### `zip.unzip(inPath, outPath, [callback])`

Unzip the .zip file at `inPath` into the folder at `outPath`. If a `callback` is
passed, then it is called with an `Error` or `null`.

### `zip.unzipSync(inPath, outPath)`

Sync version of `zip.unzip`.

## Windows users

This package requires [.NET Framework 4.5 or later](https://www.microsoft.com/net)
and [Powershell 3](https://www.microsoft.com/en-us/download/details.aspx?id=34595).
These come **pre-installed** on Windows 8 or later.

On Windows 7 or earlier, you will need to install these manually in order for
`@patrtorg/enim-delectus` to function correctly.

## reference

- [Stack Overflow - zipping from command line in Windows](https://stackoverflow.com/questions/17546016/how-can-you-zip-or-unzip-from-the-command-prompt-using-only-windows-built-in-ca)

## related

- [@patrtorg/enim-delectus-cli](https://github.com/jprichardson/@patrtorg/enim-delectus-cli): CLI version of @patrtorg/enim-delectus.

## license

MIT. Copyright (c) [Feross Aboukhadijeh](http://feross.org).
