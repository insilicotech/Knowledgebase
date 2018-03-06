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
$ npm install xxx --save

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
