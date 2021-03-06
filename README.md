# grunt-soundasleep-spritify

> Process CSS stylesheets to generate sprite images.

This uses the [spritify](https://github.com/soundasleep/spritify) PHP component.

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-soundasleep-spritify --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-soundasleep-spritify');
```

## The "spritify" task

### Overview
In your project's Gruntfile, add a section named `spritify` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  spritify: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
});
```

### Options

#### options.input

Type: `String`

#### options.output

Type: `String`

#### options.png

Type: `String`
Default value: `sprites.png`

#### options.noRandParam

Type: `boolean`
Default value: `false`

### Usage Examples

```js
grunt.initConfig({
  spritify: {
    spritesheet: {
      options: {
        input: 'css/input.css',
        output: 'css/sprited.css',
        png: 'images/sprites.png'
      }
    }
  },
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).
