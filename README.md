Truncate [![Build Status](https://drone.io/github.com/FGRibreau/node-truncate/status.png?update)](https://drone.io/github.com/FGRibreau/node-truncate/latest) [![Downloads](http://img.shields.io/npm/dm/truncate.svg)](https://www.npmjs.com/package/truncate) [![available-for-advisory](https://img.shields.io/badge/available%20for%20advising-yes-ff69b4.svg?)](http://bit.ly/2c7uFJq) [![Twitter Follow](https://img.shields.io/twitter/follow/fgribreau.svg?style=flat)](https://twitter.com/FGRibreau)
==================

Truncate text and keeps urls safe.

## NPM
Install the module with: `npm install truncate`

## Usage

```javascript
// Browser
String.truncate("1234 http://google.com hey :)", 2) === "12..."
```

```javascript
// NodeJS
> truncate = require('truncate');
> truncate("1234 http://google.com hey :)", 4);
"1234..."
> truncate("1234 http://google.com hey :)", 4, {ellipsis:null}); // or ellipsis:''
"1234"
> truncate("1234 http://google.com hey :)", 6);
"1234 http://google.com..."
> truncate("1234 http://google.com hey :)", 100);
"1234 http://google.com hey :)"
```

## [Changelog](/CHANGELOG.md)

## Donate

I maintain this project in my free time, if it helped you please support my work via [paypal](https://paypal.me/fgribreau) or [bitcoins](https://www.coinbase.com/fgribreau), thanks a lot!

## License
Copyright (c) 2014 Francois-Guillaume Ribreau
Licensed under the MIT license.
