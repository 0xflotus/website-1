---
id: version-7.0.0-babel-plugin-syntax-async-generators
title: @babel/plugin-syntax-async-generators
sidebar_label: syntax-async-generators
original_id: babel-plugin-syntax-async-generators
---

## Example

**Syntax**

```javascript
async function* agf() {
  await 1;
}
```

```js
async function f() {
  for await (let x of y) {
    g(x);
  }
}
```

## Installation

```sh
npm install --save-dev @babel/plugin-syntax-async-generators
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["@babel/plugin-syntax-async-generators"]
}
```

### Via CLI

```sh
babel --plugins @babel/plugin-syntax-async-generators script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["@babel/plugin-syntax-async-generators"]
});
```

## References

* [Proposal: Asynchronous iteration for ECMAScript](https://github.com/tc39/proposal-async-iteration)

