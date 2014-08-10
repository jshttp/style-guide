# npm-name

[![NPM Version](https://img.shields.io/npm/v/style-guide.svg?style=flat)](https://www.npmjs.org/package/style-guide)
[![Node.js Version](https://img.shields.io/badge/node.js->=_0.8-blue.svg?style=flat)](http://nodejs.org/download/)
[![Build Status](http://img.shields.io/travis/expressjs/vary.svg?style=flat)](https://travis-ci.org/expressjs/style-guide)
[![Coverage Status](https://img.shields.io/coveralls/expressjs/style-guide.svg?style=flat)](https://coveralls.io/r/expressjs/style-guide)

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
var express = require('express')
var module  = require('npm-name')

var app = express()
app.use(module())
```

### module(options)

#### Options

- `option1`    - asdf. (default `true`)
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

## Examples

Full examples go here.

### [License (type)](LICENSE)
