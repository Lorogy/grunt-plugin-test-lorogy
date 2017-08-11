# grunt-lorogy

> self-created grunt plugin,by enviroment  only

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-lorogy --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-lorogy');
```

## The "lorogy" task

### Overview
In your project's Gruntfile, add a section named `lorogy` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  lorogy: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

### Options

#### options.who 
Type: `String`
Default value: `task1`

指明哪一个来放在js代码前

#### options.commentSymbol
Type: `String`
Default value: `//`

指明拼接到js代码中使用的注释符

### Usage Examples

#### Default Options
```js

grunt.initConfig({
  lorogy: {
    options: {
    'who':'task1',
    'commentSymbol':'//'
    },
    dist:['example/*.js']
  },
})
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
2017-8-11&&nbsp;&nbsp;&nbsp;&nbsp;v0.0.1&nbsp;&nbsp;&nbsp;&nbsp;init

## License
Copyright (c) 2017 lorogy. Licensed under the MIT license.
