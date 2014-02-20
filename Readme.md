*This repository is a mirror of the [component](http://component.io) module [segmentio/alias](http://github.com/segmentio/alias). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/segmentio-alias`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# alias

  Change an object's keys to new keys.

## Installation

    $ component install segmentio/alias
    $ npm install segmentio/alias

## Example

By dictionary:

```js
var alias = require('alias');
var obj = { a: 1 };

alias(obj, { a: 'b' });
// { b: 1 }
```

By function:

```js
var alias = require('alias');
var obj = { a: 1 };

alias(obj, function (key) { return key + key; });
// { aa: 1 }
```

## API

### alias(object, dictionary || convert)

  Changes an `object`'s keys using a `dictionary` of new key names, or a `convert` function.

## License

  MIT
