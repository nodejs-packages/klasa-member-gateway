# klasa-member-gateway

this is only a temporary fix and once it stops working fully I'll remove it.

[![Build Status](https://dev.azure.com/dirigeants/klasa/_apis/build/status/dirigeants.klasa-member-gateway?branchName=master)](https://dev.azure.com/dirigeants/klasa/_build/latest?definitionId=3&branchName=master)

Simple plugin to manage an efficient per-member settings gateway.

## Installation

```bash
# NPM
$ npm install --save nodejs-packages/klasa-member-gateway

# Yarn
$ yarn add nodejs-packages/klasa-member-gateway
```

## Setup

```js
const { Client } = require('klasa');

Client.use(require('klasa-member-gateway'));

// Modifying the Schema
Client.defaultMemberSchema
    .add('experience', 'integer', { default: 0 })
    .add('level', 'integer', { default: 0 });
```
