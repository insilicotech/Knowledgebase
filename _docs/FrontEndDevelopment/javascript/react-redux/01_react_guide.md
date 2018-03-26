---
title: "Guide of React"
permalink: /docs/FrontEndDevelopment/React/introduction/
excerpt: ""
last_modified_at: 2018-03-26T08:28:04+09:00
toc: false
---

# React Tutorial

## DevOps Configuration

### Requirement

-   npm > 5.2 (for npx)

### Starter-Kit

-   create-react-app (official starter-kit)

### Installation

```bash
#
$ npm install -g create-react-app
$ npx create-react-app my-app
$ cd my-app
$ npm start
```

### Manual Create React Project

```bash
# 1. Init a javascript project, and add react relative packages.
$ yarn init -y
$ yarn add react react-dom

# 2. Enable ES6 and JSX (via Babel)
$ yarn add babel-preset-env babel-preset-react
$ touch  .babelrc
# Add following content to `.babelrc`
{
  "presets": ["env","react"]
}
```

## React Project Boilerplate

1. Git Repository
   -  Git Repository
   -  Readme
   - .gitignore
2. Project Directory Structure
   ```
   react-boilerplate
    |--dist
       |--public
    |--src
       |--client
       |--server
```
3. Node packages
4. Babel
5. Webpack
6. Test
7. React setup


## Reference

### Devops

-   [React Boilerplate](https://medium.freecodecamp.org/how-to-build-your-own-react-boilerplate-2f8cbbeb9b3f)
-   [WebPack for React](https://medium.freecodecamp.org/learn-webpack-for-react-a36d4cac5060)
- [Rekit](https://medium.freecodecamp.org/using-rekit-studio-in-an-existing-react-project-39713d9667b)
