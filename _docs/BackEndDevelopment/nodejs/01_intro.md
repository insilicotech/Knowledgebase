---
title: "Introduction of NodeJS"
permalink: /docs/BackEndDevelopment/NodeJS/introduction/
excerpt: ""
last_modified_at: 2018-01-02T16:28:04-05:00
toc: false
---

## Working Directory

```bash
/IST
└── Source/
     └── javascript
           └── nodejs
                 └── workflow
```

## Prepare node packages

``` bash
# Initial Project & Install dependent packages
$ npm init
$ npm install normalize --save

# Development Dependencies
$ npm config set prefix /usr/local
$ npm install gulp-cli --global
$ npm install gulp-cli --save-dev

$ npm install gulp-watch --save-dev
$ npm install gulp-postcss --save-dev
$ npm install gulp-sass --save-dev
$ npm install autoprefixer --save-dev
$ npm install postcss-simple-vars --save-dev
$ npm install postcss-nested --save-dev
$ npm install postcss-import --save-dev

$ npm link gulp
```
## Gulp Workflow

### Simple Gulp task (include 'gulp-watch')

Sample task file: `gulpfile.js`

```js
var gulp  = require('gulp'),
    watch = require('gulp-watch');

gulp.task('default', function(){
  console.log('Hello Gulp!')
})

gulp.task('html', function(){
  console.log('./app/index.html modified.');
});

gulp.task('watch', function(){
  var html = ['html'];
  gulp.watch('./app/index.html', html);
});

```

### Gulp Workflow for CSS

First, prepare the `.sass-lint.yml` file.

```yml
options:
  formatter: stylish
files:
  include: '**/*.s+(a|c)ss'
rules:
  # Extends
  extends-before-mixins: 1
  extends-before-declarations: 1
  placeholder-in-extend: 1

  # Mixins
  mixins-before-declarations: 1

  # Line Spacing
  one-declaration-per-line: 1
  empty-line-between-blocks: 1
  single-line-per-selector: 1

  # Disallows
  no-attribute-selectors: 0
  no-color-hex: 0
  no-color-keywords: 1
  no-color-literals: 1
  no-combinators: 0
  no-css-comments: 1
  no-debug: 1
  no-disallowed-properties: 0
  no-duplicate-properties: 1
  no-empty-rulesets: 1
  no-extends: 0
  no-ids: 1
  no-important: 1
  no-invalid-hex: 1
  no-mergeable-selectors: 1
  no-misspelled-properties: 1
  no-qualifying-elements: 1
  no-trailing-whitespace: 1
  no-trailing-zero: 1
  no-transition-all: 1
  no-universal-selectors: 0
  no-url-domains: 1
  no-url-protocols: 1
  no-vendor-prefixes: 1
  no-warn: 1
  property-units: 0

  # Nesting
  declarations-before-nesting: 1
  force-attribute-nesting: 1
  force-element-nesting: 1
  force-pseudo-nesting: 1

  # Name Formats
  class-name-format: 1
  function-name-format: 1
  id-name-format: 0
  mixin-name-format: 1
  placeholder-name-format: 1
  variable-name-format: 1

  # Style Guide
  attribute-quotes: 1
  bem-depth: 0
  border-zero: 1
  brace-style: 1
  clean-import-paths: 1
  empty-args: 1
  hex-length: 1
  hex-notation: 1
  indentation: 1
  leading-zero: 1
  max-line-length: 0
  max-file-line-count: 0
  nesting-depth: 1
  property-sort-order: 1
  pseudo-element: 1
  quotes: 1
  shorthand-values: 1
  url-quotes: 1
  variable-for-property: 1
  zero-unit: 1

  # Inner Spacing
  space-after-comma: 1
  space-before-colon: 1
  space-after-colon: 1
  space-before-brace: 1
  space-before-bang: 1
  space-after-bang: 1
  space-between-parens: 1
  space-around-operator: 1

  # Final Items
  trailing-semicolon: 1
  final-newline: 1
```

Next, the samle sass file.
```sass
// 1. Plain css
body {
  padding: 25px;
  margin: 25px;
  columns: 300px 2;
}

// 2. Variable
$MainColor: #1160c7
h1 {
  color: $MainColor;
}

// 3. Nested
section {
  a {
    color: $MainColor;
    margin: 15px;
  }
}
```

### Reference

* [PostCSS – Sass Killer or Preprocessing Pretender?](https://ashleynolan.co.uk/blog/postcss-a-review)
* [PostCSS: Life after Sass](https://www.bignerdranch.com/blog/postcss-life-after-sass/)
* [Stackshare: SASS vs. PostCSS vs. Less](https://stackshare.io/stackups/less-vs-postcss-vs-sass)
