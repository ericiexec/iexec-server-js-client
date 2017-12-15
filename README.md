# iexec-server-js-client
JS client lib to interact with iExec REST API

# Test
```bash
npm test
```


# Example
```js
const createIEXECClient = require('iexec-server-js-client')

const iexec = createIEXECClient({
  login: '',
  password: '',
  hostname: 'localhost',
  port: '9443',
})

iexec.getApps().then(console.log) // print apps from server
```
