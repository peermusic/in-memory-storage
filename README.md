# Storage in memory

A tiny module to only read/write localStorage whenever neccessary, and else keeping data in memory. It also handles converting data so you can pass objects/arrays into it.

## Install

```sh
npm install https://github.com/peermusic/in-memory-storage
```

```js
var storage = require('in-memory-storage')
```

For reference see the [Browserify Handbook](https://github.com/substack/browserify-handbook#how-node_modules-works).

## Usage

```js
var storage = require('in-memory-storage')

// Read a key from memory or localStorage, with an optional default
storage.get('key', {})

// Set a key in memory and localStorage
storage.set('key', {id: 1, name: 'Test'})

// Remove a key from memory and localStorage
storage.remove('key')
```
