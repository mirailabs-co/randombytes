# randombytes

**WHY FORKED?**
Fork this for publishing latest code because the main repo hasn't been released the latest version yet
On browser, the **global** is not compatible somewhere, so we need to change to **globalThis**

randombytes from node that works in the browser. In node you just get crypto.randomBytes, but in the browser it uses .crypto/msCrypto.getRandomValues

```js
var randomBytes = require("randombytes");
randomBytes(16); //get 16 random bytes
randomBytes(16, function (err, resp) {
  // resp is 16 random bytes
});
```
