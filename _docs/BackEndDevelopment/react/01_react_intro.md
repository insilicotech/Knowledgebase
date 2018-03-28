---
title: "Introduction of React"
permalink: /docs/BackEndDevelopment/React/introduction/
excerpt: ""
last_modified_at: 2018-01-02T16:28:04-05:00
toc: false
---

# Guide of React-Redux

## 環境構築（Configuration）

### Atom

```bash
# Install atom packages
$ apm install linter linter-eslint react linter-stylelint

# Install local packages
$ yarn add --dev eslint babel-eslint eslint-plugin-react stylelint
```

## Startup a Project

```bash
# Approach 1. via Yoman generator
$ npm install -g yo
$ npm install -g generator-react-fullstack
$ yo react-fullstack
```

> HTML as a ** Projection ** of app state, but not as source of truth.
>
> React is a pattern for organizing a UI that can transcend the DOM,
> front-end applications, and even the web platform

## Part II

Use JSX to mix UI logic with the actual UI elements in a declarative way.

### Conditional Render

```javascript
const condition = true;

const App = () => (
  <div>
    <h1>This is always visible</h1>
    {
      condition && (
        <div>
          <h2>Show me</h2>
          <p>Description</p>
        </div>
      )
    }
  </div>
);
```

### Destructuring Props

Transforming components is much easier using this pattern.

```javascript
const Details = ( { name, language } ) => (
  <div>
    <p>{ name } works with { language }</p>
  </div>
);

class Details extends React.Component {
  render() {
    const { name, language } = this.props;
    return (
      <div>
        <p>{ name } works with { language }</p>
      </div>
    )
  }
}
```

### Provider Pattern

The top level component — called Provider — sets some values on the context. The child components — called Consumers — will grab those values from the context.

The current context syntax is a bit strange, but the upcoming version is implementing this exact pattern.

```javascript

```

### High Order Component

-   [User a Render Prop](https://cdb.reacttraining.com/use-a-render-prop-50de598f11ce)

## Reference

-   [React Starter Kit](https://github.com/kriasoft/react-starter-kit)
-   [Why Redux](https://medium.freecodecamp.org/exploring-the-what-and-the-why-of-redux-6faadab4768b)
-   [FreecodeCamp: Evolving Patterns in React 16](https://medium.freecodecamp.org/evolving-patterns-in-react-116140e5fe8f)
-   [ES2015 Features used in Ract](https://www.saltycrane.com/blog/2016/03/es6-features-used-react-development/)
