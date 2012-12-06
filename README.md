# backbone-router

  Backbone Router [Component](https://github.com/component/component/wiki/Components)

## Installation

    $ component install spini/backbone-router

## History stuff

It provides `Router.history` instead of `Backbone.history`

## Example

```js

var Router = require('spini-backbone-router');

var Workspace = Router.extend({

  routes: {
    "help":                 "help",    // #help
    "search/:query":        "search",  // #search/kiwis
    "search/:query/p:page": "search"   // #search/kiwis/p7
  },

  help: function() {
    ...
  },

  search: function(query, page) {
    ...
  }

});

```

# instantiate your Router

```

var myrouter = new Router(options);

```


# and then start history

```

Router.history.start({pushState: true});

// or

Router.history.start();

```


## API

See documentation for [Backbone.Router](http://backbonejs.org/#Router)

## License

[MIT](https://github.com/spini/backbone-router/blob/master/LICENSE)
