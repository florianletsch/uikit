# UIkit

UIkit is a lightweight and modular front-end framework for developing fast and powerful web interfaces.

* Homepage: [http://www.getuikit.com](http://www.getuikit.com)
* Twitter: [@getuikit](http://twitter.com/getuikit)

## Getting started

Download the [latest release](https://github.com/uikit/uikit/zipball/master) or clone the repo, `git clone git://github.com/uikit/uikit.git`.

## Bug tracker

Report bugs on [UIkit Issues](https://github.com/uikit/uikit/issues?state=open).

## Developers

First of all, install [Node](http://nodejs.org/). We use [Grunt](http://gruntjs.com) to build UIkit. If you haven't used Grunt before, you need to install the `grunt-cli` package as a global install.

```
npm install -g grunt-cli
```

If you haven't done so already, clone the UIkit git repo.

```
git clone git://github.com/uikit/uikit.git
```
Install the Node dependencies.

```
cd uikit
npm install
```

Run `grunt` to lint, build and minify the release.

```
grunt
```

The built version of UIkit will be put in the `/dist` subdirectory.

Enter the following, so Grunt will watch your working directory and compile LESS files automatically everytime you hit save.

```
grunt watch
```

### For SCSS lovers

If you want to work with SCSS instead of LESS, we've included a basic converter. Run
the grunt task `make-scss` and you will have `/src/scss` filled with the SCSS files. Also, you
will find a theme in `themes/default/default-scss` to get you started.

```
grunt make-scss
``

To kick off compiling SCSS simply compile `uikit.scss` included in the theme
folder and drop the output in the dist folder. Depending on your preferred
SCSS process you might want to run:

```
sass themes/default/default-scss/uikit.scss > dist/css/uikit.css
sass themes/default/default-scss/uikit.scss --style compressed > dist/css/uikit.min.css
```


## Versioning

UIkit is maintained by using the [Semantic Versioning Specification (SemVer)](http://semver.org).

## Credits

We built UIkit using popular open source projects.

* jQuery ([MIT License](http://opensource.org/licenses/MIT))
* normalize.css ([MIT License](http://opensource.org/licenses/MIT))
* FontAwesome ([CC BY 3.0 License](http://creativecommons.org/licenses/by/3.0/))

## Copyright and license

Copyright 2013 [YOOtheme](http://www.yootheme.com) GmbH under the [MIT license](LICENSE.md).
