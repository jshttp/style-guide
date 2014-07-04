# npmjs-name

[![NPM Version](https://badge.fury.io/js/style-guide.svg)](https://badge.fury.io/js/style-guide)
[![Build Status](https://travis-ci.org/expressjs/style-guide.svg?branch=master)](https://travis-ci.org/expressjs/style-guide)
[![Coverage Status](https://img.shields.io/coveralls/expressjs/style-guide.svg?branch=master)](https://coveralls.io/r/expressjs/style-guide)


This document is a general guideline for expressjs repo readme's.

Documentation of basic and important functionality should always be included in the readme.

    make sure to highlight all code with ```syntax
    e.g. ```js or ```bash

### Install

```bash
$ npm install <module>
```

## API

```js
var express = require('express')
var example = require('example')

var app = express()
app.use(example())
```

### Main(options)

#### Options

- `option1`    - asdf. (default `true`)
- `option2`    - cats.
- `option10`   - always 42.
- `option9000` - epic.
  - default: `this is a very long default right here`

#### Sub Options

#### method(args)

Describes what this function does. As concisely as possible.

```js
Main.example(args)
```

### existing_object.object

#### Object.method(args)

Description

```js
existing_object.object.example(args)
```

#### Object.property

Description

```js
existing_object.object.property // => example value from description
```

## Examples

Full examples go here.

## License (type)

License or link to LICENSE file.
