# @remarkablemark/test

[GitHub Package](https://docs.github.com/packages) test

## Prerequisites

Update `.npmrc`:

```
@remarkablemark:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
```

Create a [token](https://github.com/settings/tokens):

- `read:packages`

Add to your `.zshrc` or `.bashrc`:

```sh
export GITHUB_TOKEN=ghp_xxx
```

## Install

```sh
npm install @remarkablemark/test
```

## Usage

```js
const { hello } = require('@remarkablemark/test');

console.log(hello()); // 'Hello, world!'
```
