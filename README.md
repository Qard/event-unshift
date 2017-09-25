# event-unshift

[![Greenkeeper badge](https://badges.greenkeeper.io/Qard/event-unshift.svg)](https://greenkeeper.io/)

Add event listeners before existing listeners.

### Install

```sh
npm install event-unshift
```

### Usage

```js
var patch = require('event-unshift')
patch(emitter)
emitter.unshift('error', function (error) {
  // Listen to errors before other listeners handle them, and don't
  // change default behavior of crashing when there's no real listeners.
})
```
