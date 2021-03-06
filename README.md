# employer-style-grid

A stack-agnostic SASS library providing a framework-agnostic, [Neat](http://neat.bourbon.io/)-based grid system intended for the Employer experience.

### Consumption

Add and install with Yarn:

```sh
$ yarn add employer-style-grid
```

Now, import `sass/directives/00_variables/grid-settings` after [Bourbon](http://bourbon.io/) and [Neat](http://neat.bourbon.io/) in your main `application.scss`. Then, import `sass/base`. For example:

```scss
@import 'bourbon/app/assets/stylesheets/bourbon';
@import 'bourbon-neat/app/assets/stylesheets/neat-helpers';
@import 'bourbon-neat/app/assets/stylesheets/neat';
@import 'employer-style-grid/sass/base';

@import 'your-app';
```

You can now use [Neat mixins](http://thoughtbot.github.io/neat-docs/latest/) and the provided breakpoints (see `_grid-settings.scss`), mixins and selectors.

### What's included

At the moment, only uncompiled SASS source files are available for consumption. That means your application will need to perform the precompilation, whether it be through Webpack, Gulp, Grunt, Rails asset pipeline, etc. Do note that `employer-style-grid` simply wraps around and depends upon [Neat](http://neat.bourbon.io/) to actually power its grid system.

### Contributing

#### Updating the Version

After your PR is merged, update the [semantic version number appropriately](http://semver.org/), add a [release](https://github.com/cb-talent-development/employer-style-grid/releases) and `publish` via Yarn or npm.

Then update the `package.json` file in your project with the new version:

```json
  "dependencies": {
    "employer-style-grid": "^2.0.0"
  }
```

### Future

- Implement build process to compile CSS into `dist` for easy consumption
