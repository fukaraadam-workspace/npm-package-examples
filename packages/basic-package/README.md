# Simplest Package

Just to show the simplest possible package. Followed [this tutorial](https://www.freecodecamp.org/news/how-to-create-and-publish-your-first-npm-package/).

## Local Usage

You can run `npm link` from this subdirectory to put this package into your global npm modules (revertable it with `npm unlink @fukaraadam-workspace/basic-package`). Then, you can use it in other projects with `npm link @fukaraadam-workspace/basic-package` command (revertable by removing node_modules) and following code:

```js
const helloNpm = require('@fukaraadam-workspace/basic-package');

console.log(helloNpm());
```

or, above code can be directly used in root directory of this monorepo with `node ./basic-script.js` command (without npm link).

## Publishing

1. `npm login` (if not logged in)
2. `npm publish` for simple packages. `npm publish --access public` for scoped packages like this one.
