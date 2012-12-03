# backbone-router

  Backbone Router [Component](https://github.com/component/component/wiki/Components)

## Installation

    $ component install spini/backbone-router

## Example

```js

var Router = require('backbone-router');

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

## API

See documentation for [Backbone.Router](http://backbonejs.org/#Router)

## License

[MIT](https://github.com/spini/backbone-router/blob/master/LICENSE)