# findall-pkg-mgr

It finds all package-managers installed in the system. It finds them without requiring any external dependency.

## Why?

Well, sometimes you might want to install dependencies dynamically based on the package-managers. Some folks prefer [yarn](https://yarnpkg.com/) over [npm](https://www.npmjs.com/).

## Supported Packages

1. npm
2. yarn

## How to

1. installation:
```bash
npm install --save findall-pkg-mgr
```
2. Use as a module
```javascript
const findAll = require("findall-pkg-mgr");
const pkg_mgrs = findAll();

console.log(pkg_mgrs); // [ 'npm', 'yarn' ]
```