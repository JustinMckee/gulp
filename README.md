# gulp
A gulp workflow for with Sass, javaScript ES6 support, PHP, image/asset compression

# Getting Started

1. $ `npm install`
2. In gulpfile.js, replace LOCALHOST with your proxy url so browsersync can hot reload


# Tasks Available

## Images

$ `gulp images`

Compresses images found in assets/images and sub-directories and moves to dist/images/ while keeping same directory structure

## Styles

$ `gulp styles`

Minifies, creates sourcemap, adds vendor prefixes, for all partials that have been created & imported into assets/styles/main.scss. Moves result to dist/styles/main.css and dist/styles/main.css.map

## Scripts

$ `gulp scripts`

ES6 Support with Babel, Uglifies, concatenates all files in assets/scripts and sub-directories. Moves result to dist/styles/main.js

## Watch

$ `gulp watch`

Listens for any changes to PHP files outside of assets directory and any change within assets directory. Uses browsersync to reload.

## Default

$ `gulp`

Runs the following tasks: Images, Styles, Scripts
