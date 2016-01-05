Genesis Sample Theme with Sass
===

This fork includes modern development tools like Grunt, Sass, PostCSS, and Bourbon. I *try* to keep it up to date with Genesis 2.0+ development. Your pull requests are welcome. Now, go get Sassy!

## Features
* [Grunt](https://github.com/gruntjs/grunt)
* [Sass](https://github.com/sass/node-sass) (LibSass)
* [PostCSS](https://github.com/postcss/postcss)
* [Bourbon](http://bourbon.io/)
* [LiveReload](https://github.com/livereload/LiveReload)
* Image optimization
* Script linting and CSS minifcation

## Pre-Installation

Basic knowledge of the command line and the following must be installed on your local machine:

* Node [http://nodejs.org/](http://nodejs.org/)
* Grunt CLI `npm install -g grunt-cli`

## Installation

[Download](https://github.com/gregrickaby/genesis-sample/archive/master.zip) or [clone](https://github.com/gregrickaby/genesis-sample.git) this repository and place it into your theme directory:

```bash
wordpress/wp-content/themes/genesis-sample
```

Using the terminal, navigate to your theme directory:

```bash
cd wordpress/wp-content/themes/genesis-sample
```

Install Grunt dependencies:

```bash
npm install
```

![How to use Grunt](https://dl.dropbox.com/s/hic5rpb6b5kv4i2/genesis-sample-theme-setup.gif?dl=0)

## Usage

```bash
grunt watch
```

Watch for changes and automatically refresh your browser using LiveReload.

```bash
grunt styles
```
Compile Sass, autoprefix, and then create a production ready stylesheet.

```bash
grunt javascript
```

Concatenate scripts and create a production ready script.

```bash
grunt imageminnewer
```

Optimize images located in `/images`

```bash
grunt
```

Will run all tasks mentioned above.

## Notes

###Sass Mixins

[Bourbon](http://bourbon.io/) is included! Now there is a large [library of Sass mixins](http://bourbon.io/docs/) that you can tap into.

###Javascript

All scripts placed into `/concat` will be concatenated and placed into `project.js`.

### Script Management

To load a development version (unminified) of styles and scripts add this to `wp_config.php`

```bash
define('SCRIPT_DEBUG', TRUE);
```

To load a production ready (minified) version of styles and scripts add this to `wp_config.php`

```bash
define('SCRIPT_DEBUG', FALSE);
```

## Support

* For Genesis support, please visit [http://my.studiopress.com/help/](http://my.studiopress.com/help/)
* For support with this theme, visit [https://github.com/gregrickaby/genesis-sample/issues](https://github.com/gregrickaby/genesis-sample/issues)
