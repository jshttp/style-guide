# npm-name

[![NPM Version](https://img.shields.io/npm/v/style-guide.svg?style=flat)](https://www.npmjs.org/package/style-guide)
[![NPM Downloads](https://img.shields.io/npm/dm/style-guide.svg?style=flat)](https://www.npmjs.org/package/style-guide)
[![Node.js Version](https://img.shields.io/badge/node.js->=_0.8-brightgreen.svg?style=flat)](http://nodejs.org/download/)
[![Build Status](http://img.shields.io/travis/expressjs/style-guide.svg?style=flat)](https://travis-ci.org/expressjs/style-guide)
[![Coverage Status](https://img.shields.io/coveralls/expressjs/style-guide.svg?style=flat)](https://coveralls.io/r/expressjs/style-guide)


> #### You can directly copy this folder to create a new module!

> NOTE: The "files" in package.json is a whitelist you may have to add to.


This document provides a general guideline for creating a README in an [expressjs](https://github.com/expressjs) repository.

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
