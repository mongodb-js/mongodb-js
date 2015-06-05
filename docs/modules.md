# Modules We Use

Here is a rundown of some of the modules we love and use.

## [Gulp][gulp]

[Gulp][gulp] is a build tool like grunt or
broccoli, or Make and scons if you don't usually work with JS. Gulp is
different from other JS tools in that it is streams centric and just
javascript. Unlike grunt, you don't have massive config objects you must
conform to; it takes a code over configuration approach much like Make.
If you're interested in learning more,
[here is a very detailed example][gulp-intro].

## [Jade][jade]

[Jade][jade] is our templating language
of choice.  Jade is great because:

- light enough to use on the client via browserify
- robust enough to use on the server (e.g. support for layouts and blocks)
- whitespace significant -> no "I forgot to close a tag" bugs
- no clumsy separation and helper assignment like handlebars (<3 mixins!)

## [LESS][less]

CSS is compiled from [LESS][less] files, which is great because:

- Use real variables
- File imports
- Declarative property nesting
- Source map support
- Composable with other modules

## [Browserify][browserify]

Javascript is compiled by [browserify][browserify] which works
kind of like this:

- given an entry point like `ui/app/index.js`
- follows the dependency graph opened from the entry point
- resolve dependencies from `node_modules/`
- puts all sources in one file
- each file of the graph in its own closure/scope

browserify is a huge win because we can write our client side code
exactly like our server code (minimized context switching cost) and
easily reuse modules between the server, the ui and other teams
(check out the [mongodb.js keyword][mongodb.js] on npm).

For more details, here are some slides from a
[talk @ Mongodb][browserify talk]
on npm and browserify.

## [Ampersand.js](http://ampersandjs.com/)

Highly modular, loosely coupled, non-frameworky framework for building advanced
JavaScript apps that is an evolution of Backbone.js that maximizes simplicity:

- Everything is a CommonJS module.
- Everything is installed via npm.
- Everything is MIT licensed.
- Trusted versioning with semver.
- Modern browsers by default; unapologetically supporting only IE9+.
- The browser is a runtime, not a document viewer.

## [jshint](http://jshint.com)

JSHint is a program that flags suspicious usage in programs written in JavaScript.
The core project consists of a library itself as well as a CLI program
distributed as a Node module.

## [jsfmt](https://github.com/rdio/jsfmt)

For formatting, searching, and rewriting JavaScript. Analogous to
[gofmt](http://golang.org/cmd/gofmt/).

## [sweet.js](http://sweetjs.org/)

 Define your own hygienic macros of languages like Scheme and Rust in your
 modules to spend less time on the keyboard.

## [express](http://expressjs.com/)

Express is a minimal and flexible Node.js web application framework that
provides a robust set of features for web and mobile applications.

## [mocha](http://mochajs.org)

A simple and ubiquitous test runner for JS on any platform.

## [zuul](http://npm.im/zuul)

An amazingly easy way to test your javascript in browsers. Start testing your
code in seconds locally and move to cloud based browsers seamlessly for
better coverage.

[nodejs]: http://nodejs.org/
[mongodb]: http://www.mongodb.org/downloads
[less]: http://lesscss.org
[gulp]: http://gulpjs.com
[bootstrap]: http://getbootstrap.com
[coffeescript]: http://coffeescript.org
[mocha]: http://visionmedia.github.io/mocha/
[jade]: http://github.com/visionmedia/jade
[browserify]: http://browserify.org
[font-awesome]: http://fortawesome.github.io/Font-Awesome/

[mongodb.js]: https://www.npmjs.org/browse/keyword/mongodb.js
[browserify talk]: http://imlucas.github.io/talks/mongo_052014/static/index.html
[patternlib]: http://10gen.github.io/mongoscope/patternlib.html
[less-variables]: http://10gen.github.io/mongoscope/patternlib.html#less-variables
[gulp-intro]: http://julienrenaux.fr/2014/05/25/introduction-to-gulp-js-with-practical-examples/
