# npm-name

[![NPM Version][npm-image]][npm-url]
[![NPM Downloads][downloads-image]][downloads-url]
[![Node.js Version][node-version-image]][node-version-url]
[![Build Status][travis-image]][travis-url]
[![Test Coverage][coveralls-image]][coveralls-url]


> #### This folder is a copyable template for creating new modules!

> NOTE: The "files" in package.json is a whitelist you may have to add to.

When writing content for a README, keep these two guidelines in mind:

- always describe basic functionality above `Installation`.

- always specify a language when using code blocks.

```
    // examples of a language include javascript and bash
    ```[language]
      [code]
    ```
```

## Installation

```bash
$ npm install <npm-name>
```

## API

```js
var Module = require('npm-name')
```

## Module(options)

```js
var module = Module({
  // sample options
}))
```

#### Options

- `option1`    - asdf. (default: `true`)
- `option2`    - cats.
- `option10`   - always 42.
- `option9000` - epic.
  - default: `this is a very long default right here`

#### Sub Options

#### module.method(args)

As concisely as possible, describe the purpose of this function.

```js
module.method(args)
```

### existing_object.object

#### Object.method(args)

Add a description for this method.

```js
existing_object.object.example(args)
```

#### Object.property

Add a description for this property.

```js
existing_object.object.property // => example value from description
```

## Example(s)

```js
// Full examples go here.
```

## [MIT Licensed](LICENSE)

[npm-image]: https://img.shields.io/npm/v/{{NAME}}.svg?style=flat
[npm-url]: https://npmjs.org/package/{{NAME}}
[node-version-image]: https://img.shields.io/node/v/{{NAME}}.svg?style=flat
[node-version-url]: http://nodejs.org/download/
[travis-image]: https://img.shields.io/travis/jshttp/{{NAME}}.svg?style=flat
[travis-url]: https://travis-ci.org/jshttp/{{NAME}}
[coveralls-image]: https://img.shields.io/coveralls/jshttp/{{NAME}}.svg?style=flat
[coveralls-url]: https://coveralls.io/r/jshttp/{{NAME}}?branch=master
[downloads-image]: https://img.shields.io/npm/dm/{{NAME}}.svg?style=flat
[downloads-url]: https://npmjs.org/package/{{NAME}}
