# Code

NodeJS toolkit.

Add a globally available toolkit to your NodeJS application.

### Install

`npm i code`

### Usage

Code can be included manually or automatically for each application, or system wide.

#### Include it manually

Currently Code is just a wrapper for the [NodeJS extras library.](https://github.com/eldoy/extras)

Requiring Code will add it to the global object:
```js
require('code')

// Use Code, everything in extras are available
Code.read()
Code.write()
// ... and lots more
```

See the `extras` documentation for details.


#### Include automatically

Use the `-r` option when you run the `node` command:

```
node -r './node_modules/code' app.js
```

#### Include system wide

If you want to add it globally in all your node apps without installing anything, first install Code globally:

```js
npm i -g code
```

then add this to your `.zshrc` and reload your shell:

```
NODE_OPTIONS='--require "code"'
```

The Code object should now be available in all your apps.

MIT Licensed. Enjoy!
