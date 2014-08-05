# npm-name

[![NPM Version](https://badge.fury.io/js/style-guide.svg)](https://badge.fury.io/js/style-guide)
[![Build Status](https://travis-ci.org/expressjs/style-guide.svg?branch=master)](https://travis-ci.org/expressjs/style-guide)
[![Coverage Status](https://img.shields.io/coveralls/expressjs/style-guide.svg?branch=master)](https://coveralls.io/r/expressjs/style-guide)

This document provides a general guideline for creating a README in an ExpressJS repository. 

When writing content for a README, keep these two goals in mind: 

- always include basic functionality. 

- always specifiy a language when using code blocks.

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
var npmName = require('npm-name')

var app = express()
app.use(npmName())
```

### npmName(options)

#### Options

- `option1`    - asdf. (default `true`)
- `option2`    - cats.
- `option10`   - always 42.
- `option9000` - epic.
  - default: `this is a very long default right here`

#### Sub Options

#### npmName.method(args)

As concisely as possible, describe the purpose of this function. 

```js
npmName.method(args)
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
existing_object.object.property  // => example value from description
```

## Examples

Full examples go here.

### [License (type)](LICENSE)
