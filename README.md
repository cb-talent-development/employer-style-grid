# employer-style-grid

A stack-agnostic SASS library providing a framework-agnostic, [Neat](http://neat.bourbon.io/)-based grid system intended for the Employer experience.

### Consumption

Install with Bower (from an appropriate repository)

```sh
$ bower install employer-style-grid
```

Now, import `sass/grid` after [Neat](http://neat.bourbon.io/) Helpers, and after a framework like [Bourbon](http://bourbon.io/) in your main `application.scss`. Then, import Neat. For example:

```scss
@import 'bower_components/bourbon/app/assets/stylesheets/bourbon';
@import 'bower_components/neat/app/assets/stylesheets/neat-helpers';
@import 'bower_components/employer-style-grid/sass/grid';
@import 'bower_components/neat/app/assets/stylesheets/neat';

@import 'your-app';
```

You can now use [Neat mixins](http://thoughtbot.github.io/neat-docs/latest/) and the provided breakpoints (see `_grid-settings.scss`).

### What's included

At the moment, only uncompiled SASS source files are available for consumption. That means your application will need to perform the precompilation, whether it be through Gulp, Grunt, Rails asset pipeline, etc. Do note that `employer-style-grid` simply wraps around, and depends upon [Neat](http://neat.bourbon.io/) to actually power its grid system.

### Future

- Implement build process to compile CSS into `dist` for easy consumption
