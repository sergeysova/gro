# GRO

## Usage


```js
const gro = require('gro')

const c = gro('ExampleName')


const gend = c.group('foo')
const tend = c.time('foo')

c.log('Executed foo')

tend()
gend()
```

```
ExampleName.foo
|   ExampleName Executed foo
|   Example.Name.foo: 0.186ms
└
```

## And

```js
const gro = require('gro')

const gend = gro.group('Foo')
gend()

const tend = gro.time('Bar')
tend()
```