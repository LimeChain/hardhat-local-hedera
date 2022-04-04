[![npm](https://img.shields.io/npm/v/hardhat-local-hedera.svg)](https://www.npmjs.com/package/hardhat-hethers) [![hardhat](https://hardhat.org/buidler-plugin-badge.svg?1)](https://hardhat.org)

# hardhat-local-hedera

[Hardhat](https://hardhat.org) plugin for integration with [local-hedera](https://github.com/LimeChain/local-hedera).

## What

This plugin brings to Hardhat the hedera package `local-hedera`, which allows you to interact with the local hedera nodes (consensus and mirror).

## Installation

```bash
npm install --save-dev 'hardhat-local-hedera'
```

And add the following statement to your `hardhat.config.js`:

```js
require('hardhat-local-hedera');
```

also be sure you've added it before `hardhat-hethers`
```js
require('hardhat-local-hedera');
require('hardhat-hethers');
```

## Tasks

This plugin creates no additional tasks.

## Environment extensions

This plugin resets the local network everytime on runtime.

## Usage

There are no additional steps you need to take for this plugin to work.

Under the hood, the plugin uses local-hedera as peer dependency, so you should be able to interact with the plugin on the fly via `npx local-hedera`.