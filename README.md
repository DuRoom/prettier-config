# DuRoom Prettier Config

DuRoom's official configuration for the Prettier code formatter.

For more info about shared Prettier configurations, [check out the Prettier documentation](https://prettier.io/docs/en/configuration.html#sharing-configurations).

## Usage

1. Install `@duroom/prettier-config` as a dev dependency:

```
npm i -D @duroom/prettier-config
yarn add -D @duroom/prettier-config
```

2. Add the `prettier` key to your `package.json`:

```jsonc
// package.json
{
  "name": "my-cool-package",
  "version": "1.0.0",
  "prettier": "@duroom/prettier-config",
  // ...
}
```

## Extending

You can extend our config with your own custom options, too. Import our config, then spread its require in a `.prettierrc.js` file.

> :warning: Make sure your `package.json` doesn't have the `prettier` key.

```js
// .prettierrc.js
module.exports = {
  ...require("@duroom/prettier-config"),
  semi: false,
};
```
