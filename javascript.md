### Rules

* Two space indention
* No trailing whitespace
* End-of-file newlines in all text files

### Guidelines

* Prefer the latest ECMAScript syntax available on the target platform(s)
* Try to keep lines less than 80 characters wide
* Use files for additional scope rather than closures
* Prefer `'` over `"` - avoid escaping quotations

#### Prefer no semicolons

Except when necessary, such as in `for(;;){}`.

Do not argue about semicolons or the lack thereof.
There are better, more important fights to fight.

#### Opening braces on statement line

```js
function () {
  // =^.^=
}
```

#### One var per line

```js
var one = 1
var two = 2
```

#### Use Function Declarations

```js
function fn() {}
```

Exceptions:

- Exporting - `export.fn = function () {}`
- Conditionals - `var fn = a ? function () {} : function () {}`

#### Spaces around function definition

```js
function fn(a, b) {}
```

#### Spaces around operators

```js
if () {} else {}
switch () {}

for (a; b >= c; c + d / e) {}

// ++ -- ~ are exceptions
a++
--b
~array.indexOf('c')
```

#### Spaces only after commas or semicolons in arguments

```js
function fn(a, b) {}
if (a, b, c) {}
for (a; b; c) {}
```

#### Multiline arrays and objects

If the attributes are likely to change,
define each element on a separate line.

Add trailing commas to multiline definitions.

```js
var thing = {
  not_changing: ['c', 'a', 't'],
  might_change: [
    'bitcoin',
  ]
  a: 'z',
  b: 'y',
}
```

#### Declare functions outside of arrays

```js
parallel([fn1, fn2], callback)

function fn1() {}
function fn2() {}
```

#### Use short or 3-character names when readability is preserved

```js
var req = http.get(function (res) {
  // still makes sense
})
```

#### Avoid statements starting with a `[` or `(`

If necessary, prepend with a semicolon.

```js
;[].forEach()
;(function () {})()
```

### Code Order

Code should philosophically be ordered:

- From high level to lower level
- From public to private

Code in a single file should generally be structured in the following order:

1. Global imports - `require('lib')`
2. Relative imports - `require('./src')`
3. Variables - `var a = 1`
4. Exports - `module.exports = Main`
5. Main - `function Main() {}`
6. Prototype Properties - `Main.prototype.something = true`
7. Utilities - `function add(a, b) {return a + b}`
