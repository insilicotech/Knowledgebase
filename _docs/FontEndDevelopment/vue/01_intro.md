---
title: "Introduction of Vue"
permalink: /docs/FontEndDevelopment/Vue/introduction/
excerpt: "How to quickly install and setup Minimal Mistakes for use with GitHub Pages."
last_modified_at: 2018-01-02T16:28:04-05:00
toc: false
---

## Environment Construction

###

* [Vue-Cli](https://github.com/vuejs/vue-cli)
* [Atom package: language-vue-component ](https://atom.io/packages/language-vue-component)
* [VSCode Extension: vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
* [Chrome Extension: Vue.js Devtools Extension](https://github.com/vuejs/vue-devtools)
* [Chrome Extension: DejaVue](http://dejavue.co/)


```bash
$ npm install vue
```

## Vue Introduction

A Vue instance can also be thought of as a [ViewModel](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel) in the MVVM pattern.

Vue provides two approaches for doing the two-way data binding.

* Fluid template expression (double curly brackets)
* Customized directive("v-model" Vue directve)

Vue Make you decompsing DOM junk inoto hierachical stucture implemented by following Vue Component.

* Conditional visibility controll by "v-show"
* Exclusive visibility controll by "v-if"/"v-else"
* Display elements iterativly by "v-for"/Filterby, Orderby

For interactivity, "v-on" directive(shorthand "@") for listening on DOM events.

## Features of Vue.js

* Declarative Rendering

``` html
<div id="app">
{% raw %}  {{ message }} {% endraw %}
</div>
```

``` javascript
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue!'
  }
});
```

* Dynamic Data-Binding

~~~ html
<div id="app2">
    <span v-bind:title="message">Hover your mouse over me a few seconds.</span>
</div>
~~~


``` javascript
var app2 = new Vue({
    el: '#app2',
    data: {
        message: 'You load this page on ' + new Date().toLocaleDateString()
    }
});

```
