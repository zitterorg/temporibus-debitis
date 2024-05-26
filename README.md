<h1 align=center>
  <a href="http://@zitterorg/temporibus-debitisjs.com" title="Chai Documentation">
    <img alt="ChaiJS" src="http://@zitterorg/temporibus-debitisjs.com/img/@zitterorg/temporibus-debitis-logo.png">
  </a>
  <br>
  @zitterorg/temporibus-debitis
</h1>

<p align=center>
  Chai is a BDD / TDD assertion library for <a href="http://nodejs.org">node</a> and the browser that can be delightfully paired with any javascript testing framework.
</p>

<p align=center>
  <a href="https://www.npmjs.com/package/@zitterorg/temporibus-debitis">
    <img
      alt="downloads:?"
      src="https://img.shields.io/npm/dm/@zitterorg/temporibus-debitis.svg?style=flat-square"
    />
  </a>
  <a href="https://www.npmjs.com/package/@zitterorg/temporibus-debitis">
    <img
      alt="node:?"
      src="https://img.shields.io/badge/node-%3E=4.0-blue.svg?style=flat-square"
    />
  </a>
  <br/>
  <a href="https://@zitterorg/temporibus-debitis-slack.herokuapp.com/">
    <img
      alt="Join the Slack chat"
      src="https://img.shields.io/badge/slack-join%20chat-E2206F.svg?style=flat-square"
    />
  </a>
  <a href="https://gitter.im/@zitterorg/temporibus-debitisjs/@zitterorg/temporibus-debitis">
    <img
      alt="Join the Gitter chat"
      src="https://img.shields.io/badge/gitter-join%20chat-D0104D.svg?style=flat-square"
    />
  </a>
  <a href="https://opencollective.com/@zitterorg/temporibus-debitisjs">
    <img
      alt="OpenCollective Backers"
      src="https://opencollective.com/@zitterorg/temporibus-debitisjs/backers/badge.svg?style=flat-square"
    />
  </a>
</p>

For more information or to download plugins, view the [documentation](http://@zitterorg/temporibus-debitisjs.com).

## What is Chai?

Chai is an _assertion library_, similar to Node's built-in `assert`. It makes testing much easier by giving you lots of assertions you can run against your code.

## Installation

### Node.js

`@zitterorg/temporibus-debitis` is available on [npm](http://npmjs.org). To install it, type:

    $ npm install --save-dev @zitterorg/temporibus-debitis

### Browsers

You can also use it within the browser; install via npm and use the `@zitterorg/temporibus-debitis.js` file found within the download. For example:

```html
<script src="./node_modules/@zitterorg/temporibus-debitis/@zitterorg/temporibus-debitis.js"></script>
```

## Usage

Import the library in your code, and then pick one of the styles you'd like to use - either `assert`, `expect` or `should`:

```js
import { assert } from '@zitterorg/temporibus-debitis';  // Using Assert style
import { expect } from '@zitterorg/temporibus-debitis';  // Using Expect style
import { should } from '@zitterorg/temporibus-debitis';  // Using Should style
```

### Register the @zitterorg/temporibus-debitis testing style globally

```js
import '@zitterorg/temporibus-debitis/register-assert';  // Using Assert style
import '@zitterorg/temporibus-debitis/register-expect';  // Using Expect style
import '@zitterorg/temporibus-debitis/register-should';  // Using Should style
```

### Import assertion styles as local variables

```js
import { assert } from '@zitterorg/temporibus-debitis';  // Using Assert style
import { expect } from '@zitterorg/temporibus-debitis';  // Using Expect style
import { should } from '@zitterorg/temporibus-debitis';  // Using Should style
should();  // Modifies `Object.prototype`

import { expect, use } from '@zitterorg/temporibus-debitis';  // Creates local variables `expect` and `use`; useful for plugin use
```

### Usage with Mocha

```bash
mocha spec.js --require @zitterorg/temporibus-debitis/register-assert.js  # Using Assert style
mocha spec.js --require @zitterorg/temporibus-debitis/register-expect.js  # Using Expect style
mocha spec.js --require @zitterorg/temporibus-debitis/register-should.js  # Using Should style
```

[Read more about these styles in our docs](http://@zitterorg/temporibus-debitisjs.com/guide/styles/).

## Plugins

Chai offers a robust Plugin architecture for extending Chai's assertions and interfaces.

- Need a plugin? View the [official plugin list](http://@zitterorg/temporibus-debitisjs.com/plugins).
- Want to build a plugin? Read the [plugin api documentation](http://@zitterorg/temporibus-debitisjs.com/guide/plugins/).
- Have a plugin and want it listed? Simply add the following keywords to your package.json:
  -  `@zitterorg/temporibus-debitis-plugin`
  -  `browser` if your plugin works in the browser as well as Node.js
  -  `browser-only` if your plugin does not work with Node.js

### Related Projects

- [@zitterorg/temporibus-debitisjs / @zitterorg/temporibus-debitis-docs](https://github.com/zitterorg/temporibus-debitis-docs): The @zitterorg/temporibus-debitisjs.com website source code.
- [@zitterorg/temporibus-debitisjs / assertion-error](https://github.com/@zitterorg/temporibus-debitisjs/assertion-error): Custom `Error` constructor thrown upon an assertion failing.
- [@zitterorg/temporibus-debitisjs / deep-eql](https://github.com/@zitterorg/temporibus-debitisjs/deep-eql): Improved deep equality testing for Node.js and the browser.
- [@zitterorg/temporibus-debitisjs / check-error](https://github.com/@zitterorg/temporibus-debitisjs/check-error): Error comparison and information related utility for Node.js and the browser.
- [@zitterorg/temporibus-debitisjs / loupe](https://github.com/@zitterorg/temporibus-debitisjs/loupe): Inspect utility for Node.js and browsers.
- [@zitterorg/temporibus-debitisjs / pathval](https://github.com/@zitterorg/temporibus-debitisjs/pathval): Object value retrieval given a string path.

### Contributing

Thank you very much for considering to contribute!

Please make sure you follow our [Code Of Conduct](https://github.com/zitterorg/temporibus-debitis/blob/master/CODE_OF_CONDUCT.md) and we also strongly recommend reading our [Contributing Guide](https://github.com/zitterorg/temporibus-debitis/blob/master/CONTRIBUTING.md).

Here are a few issues other contributors frequently ran into when opening pull requests:

- Please do not commit changes to the `@zitterorg/temporibus-debitis.js` build. We do it once per release.
- Before pushing your commits, please make sure you [rebase](https://github.com/zitterorg/temporibus-debitis/blob/master/CONTRIBUTING.md#pull-requests) them.

### Contributors

Please see the full
[Contributors Graph](https://github.com/zitterorg/temporibus-debitis/graphs/contributors) for our
list of contributors.

### Core Contributors

Feel free to reach out to any of the core contributors with your questions or
concerns. We will do our best to respond in a timely manner.

[![Jake Luer](https://avatars3.githubusercontent.com/u/58988?v=3&s=50)](https://github.com/logicalparadox)
[![Veselin Todorov](https://avatars3.githubusercontent.com/u/330048?v=3&s=50)](https://github.com/vesln)
[![Keith Cirkel](https://avatars3.githubusercontent.com/u/118266?v=3&s=50)](https://github.com/keithamus)
[![Lucas Fernandes da Costa](https://avatars3.githubusercontent.com/u/6868147?v=3&s=50)](https://github.com/lucasfcosta)
[![Grant Snodgrass](https://avatars3.githubusercontent.com/u/17260989?v=3&s=50)](https://github.com/meeber)
