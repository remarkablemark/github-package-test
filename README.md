# @remarkablemark/test

📦 [GitHub Package](https://docs.github.com/packages) test:

- [npm](https://github.com/remarkablemark/github-package-test/pkgs/npm/test)

Read the [blog post](https://remarkablemark.org/blog/2026/02/28/how-to-publish-npm-github-package/).

## Prerequisites

Update `.npmrc`:

```
@remarkablemark:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
```

Create auth [token](https://github.com/settings/tokens) with scope `read:packages` and add it to your shell config (e.g., `.zshrc`):

```sh
export GITHUB_TOKEN=ghp_xxx
```

Or do with with [GitHub CLI](https://cli.github.com/):

```sh
gh auth refresh -h github.com -s read:packages
```

```sh
echo 'export GITHUB_TOKEN=$(gh auth token)' >> ~/.zshrc
```

## Install

Install the package:

```sh
npm install @remarkablemark/test
```

## Usage

Use the package:

```js
const { hello } = require('@remarkablemark/test');

console.log(hello()); // 'Hello, world!'
```
