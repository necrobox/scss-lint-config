# @necrobox/scss-lint-config

[![npm](https://img.shields.io/npm/v/@necrobox/scss-lint-config.svg)](https://www.npmjs.com/package/@necrobox/scss-lint-config)

[Stylelint](https://stylelint.io) rules that follow our style guide for SCSS.

[По-русски](./README.ru.md)

## Installation

First, install Stylelint and postcss-scss that meet
the [peerDependencies requirements](./package.json):

```bash
npm install --save-dev stylelint postcss-scss
```

Then install the config:

```bash
npm install --save-dev @necrobox/scss-lint-config
```

## Usage

Include into a project config and pass desired [options](https://stylelint.io/user-guide/cli/):

```bash
stylelint "src/**/*.scss" --cache --config node_modules/@necrobox/scss-lint-config/.stylelintrc
```

Also you can create your own config based on this one:

```js
module.exports = {
  extends: '@necrobox/scss-lint-config/.stylelintrc.json',
  rules: [
    // your rule settings here
  ]
};
```
