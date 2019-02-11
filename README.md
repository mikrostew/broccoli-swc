# broccoli-swc
[![Build Status](https://travis-ci.org/stefanpenner/broccoli-swc.svg?branch=master)](https://travis-ci.org/stefanpenner/broccoli-swc)

Experimental SWC compiler for broccoli.

> Super-fast javascript to javascript compiler written in rust

TL;DR SWC is a alternative to babel / buble for the JS ecosystem.

* SWC Repo: https://github.com/swc-project/swc
* SWC Site: https://swc-project.github.io/

This module aims to experiment using SWC in the broccoli and ember-cli ecosystems.


## usage

### Basic via Brocfile.js or Broccoli pipeline

```js
// Brocfile.js
const swc = require('broccoli-swc');
module.exports = swc(__dirname + '/src', { swc: {/* swc options */ }); // where src/**/*.js contains ecmascript
```

### Extension / Subclassing

```js
// Brocfile.js
const swc = require('broccoli-swc');

module.exports = class CustomSWC extends swc.Plugin {
  // custom behavior 
}
```

## options:

TBD

## SWC Issues:

* https://github.com/swc-project/swc/issues/151
