# magisterjs-authcode

This package contains the authentication code used by [`magister.js`](https://github.com/simplyGits/MagisterJS).
The code can be used by installing it with npm or requested through HTTP.

`npm install @magisterjs/authcode`

```js
import authCode from '@magisterjs/authcode'

console.log(authCode);
```

```js
const request = require('request');

request('https://raw.githubusercontent.com/simplyGits/magisterjs-authcode/master/code.json', { json: true }, (err, res, code) => {
  if (err) {
    console.error(err);
  } else {
    console.log(code);
  }
});
```
