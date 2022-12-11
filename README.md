# Endo

NodeJS toolkit.

Add a globally available toolkit to your NodeJS application.

### Install

`npm i endo`

### Usage

Endo can be included manually or automatically for each application, or system wide.

#### Include it manually

Currently Endo is just a wrapper for the [NodeJS extras library.](https://github.com/eldoy/extras)

Requiring Endo will add it to the global object:
```js
require('endo')

// Use Endo
Endo.read()
Endo.write()
// ....
```

#### Include automatically

Use the `-r` option when you run the `node` command:

```
node -r './node_modules/endo' app.js
```

#### Include system wide

If you want to add it globally in all your node apps without installing anything, first install Endo globally:

```js
npm i -g endo
```

then add this to your `.zshrc` and reload your shell:

```
NODE_OPTIONS='--require "endo"'
```

The Endo object should now be available in all your apps.

MIT Licensed. Enjoy!
