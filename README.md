resin-auth
-----------

[![npm version](https://badge.fury.io/js/resin-auth.svg)](http://badge.fury.io/js/resin-auth)
[![dependencies](https://david-dm.org/resin-io/resin-auth.png)](https://david-dm.org/resin-io/resin-auth.png)
[![Build Status](https://travis-ci.org/resin-io/resin-auth.svg?branch=master)](https://travis-ci.org/resin-io/resin-auth)

Join our online chat at [![Gitter chat](https://badges.gitter.im/resin-io/chat.png)](https://gitter.im/resin-io/chat)

Resin.io session authentication utilities

Role
----

The intention of this module is to provide low level access to how a Resin.io authentication tokens are parsed and persisted.

**THIS MODULE IS LOW LEVEL AND IS NOT MEANT TO BE USED BY END USERS DIRECTLY**.

Unless you know what you're doing, use the [Resin SDK](https://github.com/resin-io/resin-sdk) instead.

Installation
------------

Install `resin-auth` by running:

```sh
$ npm install --save resin-auth
```

Documentation
-------------

The module returns a class that you use to get an instance of the auth module.

It accepts the following params:

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | options |
| options.dataDirectory | <code>string</code> | the directory to use for storage in Node.js. Ignored in the browser. |
| options.tokenKey | <code>string</code> | the key used to store the last token in the storage. |

**Example**
```js
const auth = require('resin-auth')({
	dataDirectory: '/opt/cache/resin',
	tokenKey: 'token'
})
```

Support
-------

If you're having any problem, please [raise an issue](https://github.com/resin-io/resin-auth/issues/new) on GitHub and the Resin.io team will be happy to help.

Tests
-----

Run the test suite by doing:

```sh
$ npm test
```

Contribute
----------

- Issue Tracker: [github.com/resin-io/resin-auth/issues](https://github.com/resin-io/resin-auth/issues)
- Source Code: [github.com/resin-io/resin-auth](https://github.com/resin-io/resin-auth)

Before submitting a PR, please make sure that you include tests, and that [coffeelint](http://www.coffeelint.org/) runs without any warning:

```sh
$ npm run lint
```

License
-------

The project is licensed under the Apache 2.0 license.
