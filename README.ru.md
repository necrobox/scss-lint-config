# @necrobox/scss-lint-config

[![npm](https://img.shields.io/npm/v/@necrobox/scss-lint-config.svg)](https://www.npmjs.com/package/@necrobox/scss-lint-config)

Пакет с правилами для [Stylelint](https://stylelint.io), соответствующие принятому в компании стайлгайду для SCSS-файлов.

## Установка

Сперва необходимо установить версии Stylelint и postcss-scss, удовлетворяющие требованиям, 
описанным в [peerDependencies](./package.json):

```bash
npm install --save-dev stylelint postcss-scss
```

Затем можно устанавливать сам конфиг:

```bash
npm install --save-dev @necrobox/scss-lint-config
```

## Использование

Подключить в конфиг рабочего проекта, передав необходимые [опции](https://stylelint.io/user-guide/cli/):

```bash
stylelint "src/**/*.scss" --cache --config node_modules/@necrobox/scss-lint-config/.stylelintrc
```

Помимо этого можно описать локальный конфиг проекта, основанный на этом:

```js
module.exports = {
  extends: '@necrobox/scss-lint-config/.stylelintrc.json',
  rules: [
    // доопределения правил
  ]
};
```
