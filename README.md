# Eldoy Code

NodeJS toolkit.

Add a globally available toolkit to your NodeJS application.

### Install

`npm i eldoy`

### Usage

Eldoy Code can be included manually or automatically for each application, or system wide.

#### Include it manually

Currently Eldoy Code is just a wrapper for the [NodeJS extras library.](https://github.com/eldoy/extras)

Requiring `eldoy` will add the `E` object to the global object:
```js
require('eldoy')

// Use Eldoy Code, everything in extras are available
E.read()
E.write()
// ... and lots more
```

See the `extras` documentation for details.


#### Include automatically

Use the `-r` option when you run the `node` command:

```
node -r './node_modules/eldoy' app.js
```

#### Include system wide

If you want to add it globally in all your node apps without installing anything, first install Eldoy Code globally:

```js
npm i -g eldoy
```

then add this to your `.zshrc` and reload your shell:

```
NODE_OPTIONS='--require "eldoy"'
```

The `E` object should now be available in all your apps.

MIT Licensed. Enjoy!
