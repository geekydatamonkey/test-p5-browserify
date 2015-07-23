# test-p5-browserify

1. Install browserify globally: `npm install -g browserify`
2. Run: `browserify main.js -o bundle.js`

Observe errors like:

```
Error: Cannot find module '../core/core' from '/Users/jjohnson136/dev/p5-browserify-test/node_modules/p5/lib'
    at /Users/jjohnson136/.nvm/versions/node/v0.12.5/lib/node_modules/browserify/node_modules/resolve/lib/async.js:55:21
    at load (/Users/jjohnson136/.nvm/versions/node/v0.12.5/lib/node_modules/browserify/node_modules/resolve/lib/async.js:69:43)
    at onex (/Users/jjohnson136/.nvm/versions/node/v0.12.5/lib/node_modules/browserify/node_modules/resolve/lib/async.js:92:31)
    at /Users/jjohnson136/.nvm/versions/node/v0.12.5/lib/node_modules/browserify/node_modules/resolve/lib/async.js:22:47
    at FSReqWrap.oncomplete (fs.js:95:15)
```

Changing p5 version 0.4.5 makes the error go away.
