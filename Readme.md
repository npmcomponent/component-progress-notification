*This repository is a mirror of the [component](http://component.io) module [component/progress-notification](http://github.com/component/progress-notification). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-progress-notification`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# ProgressNotification

  Progress notification component with a clean slate to build off of.

  ![progress notification component](http://f.cl.ly/items/0R0k131Q41452x1D303u/Screen%20Shot%202012-09-07%20at%2011.30.02%20AM.png)

## Installation

```
$ component install component/progress-notification
```

## Features

  - all the features of [notification](http://github.com/component/notification)

## Example

```js
var notify = require('progress-notification');

var progress = notify('Uploading maru.png');
var n = 0;
setInterval(function(){
  progress.update(n++);
}, 50);
```

## API

### notify(msg)

  Notify with the given `msg` and no title.

### notify(title, msg)

  Notify with the given `msg` and `title`.

### ProgressNotification#update(n)

  Update percentage to `n`.

### ProgressNotification#size(n)

  Update progress indicator size to `n`.

## License

  MIT
