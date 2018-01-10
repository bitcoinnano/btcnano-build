# btcnano-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install btcnano-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var bitcoreTasks = require('btcnano-build');

bitcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var bitcoreTasks = require('btcnano-build');
bitcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/bitpay/bitcore) on the main btcnano repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2015-2021 Btcnano, Inc. Btcnano is a trademark maintained by Btcnano, Inc.

