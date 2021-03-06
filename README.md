# iexec-server-js-client
[![Build Status](https://drone.iex.ec//api/badges/iExecBlockchainComputing/iexec-server-js-client/status.svg)](https://drone.iex.ec/iExecBlockchainComputing/iexec-server-js-client) [![npm version](https://badge.fury.io/js/iexec-server-js-client.svg)](https://www.npmjs.com/package/iexec-server-js-client) [![license](https://img.shields.io/github/license/iExecBlockchainComputing/iexec-server-js-client.svg)](LICENSE)

JS client lib to interact with iExec server REST API

## Ressources
 * The iExec server API doc: https://serverapi.iex.ec
 * [The iExec SDK](https://github.com/iExecBlockchainComputing/iexec-sdk)
 * The iExec main documentation: https://docs.iex.ec

## Test
```bash
npm test
```

## Example
```js
const createIEXECClient = require('iexec-server-js-client');

const iexec = createIEXECClient({ server: 'https://localhost:443' });
iexec.getCookieByJWT('my_jwt_token').then(
  iexec.getAppsUIDs().then(console.log) // print apps from server
);
```
