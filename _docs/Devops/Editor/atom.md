---
title: "Atom"
permalink: /docs/Devops/Editor/Atom/
excerpt: "How to quickly install and setup Minimal Mistakes for use with GitHub Pages."
last_modified_at: 2018-01-02T16:28:04-05:00
toc: false
---

```bash
$ apm install emmet
```

## Packages

| Category | Subject            | Details                                                                     | Installation                          |
| -------- | ------------------ | --------------------------------------------------------------------------- | ------------------------------------- |
| Syntax   | Vue                | [Language-Vue](https://atom.io/packages/language-vue)                       | $ apm install language-vue            |
|          | Markdown           | [Language-Markdown](https://atom.io/packages/language-markdown)             | $ apm install language-markdown       |
| Lint     | core               | [linter](https://atom.io/packages/linter)                                   | $ apm install lint                    |
|          | ui-default         | [linter-ui-default](https://atom.io/packages/linter-ui-default)             | $ apm install linter-ui-default       |
|          | CSS                | [linter-stylelint](https://atom.io/packages/linter-stylelint)               | $ apm install linter-stylelint        |
|          | scss               |                                                                             | `$ apm install linter-scss-lint`      |
|          | SASS               | [SASS](https://atom.io/packages/linter-sass-lint)                           | $ apm install linter-sass-lint        |
|          | Javascript         | [eslint](https://atom.io/packages/linter-eslint)                            | $ apm install linter-eslint           |
|          | Python             | [pylama](https://atom.io/packages/linter-pylama)                            | $ apm install linter-pylama           |
|          | Ruby               | rubocop                                                                     | `$ apm install linter-rubocop`        |
| Util     | Terminal           | [platformio-ide-terminal](https://atom.io/packages/platformio-ide-terminal) | $ apm install platformio-ide-terminal |
|          | Multiple Selection | [multi-cursor](https://atom.io/packages/multi-cursor)                       | $ apm install multi-cursor            |
|          | Color              | [colorpiker](https://atom.io/packages/color-picker)                         | $ apm install color-picker            |
|          | UI                 | file-icon                                                                   | $ apm install file-icons              |
|          | Help               | [ask stackoverflow](https://atom.io/packages/ask-stack)                     | `$ apm install ask-stack`             |
|          | Pane               | Pane layout Plus                                                            | `$ apm install pane-layout-plus`      |
| Vue      |                    | snippets                                                                    | `$ apm install vue-snippets`          |
|          |                    | autocomplete                                                                | `$ apm install vue2-autocomplete`     |
| Language | Elm                | [language-elm](https://atom.io/packages/language-elm)                       | `$ apm install language-elm`          |
|          |                    | elm-oracle                                                                  | `$ npm install -g elm-oracle`         |
| Editing  | Autocomplete       | autocomplete-snippets                                                       | `$ apm install autocomplete-snippets` |
| Lint     | Syntax/Format      | atom-beautify                                                               | `$ apm install atom-beautify`         |
|React | react| react `$ apm install react`|

## Setting

| Category | Item  | Setting Value    |
| -------- | ----- | ---------------- |
| UI       | Theme | isotope light    |
|          | Color | Pen Paper Coffee |

## Shutcut Keys

| Category | Task                   | Shortcut Key                    |
| -------- | ---------------------- | ------------------------------- |
| Window   | Reload Window          | `CTL + Alt + CMD + l`           |
|          | Toggle Developer Tools | `alt + CMD + i`                 |
|          | Tree View              | `CMD + ¥` or `CMD + K, CMD + b` |
| Setting  | Configure Panel        | `CTL + ,`                       |
| Editing  | Beautify               | `CTL + Alt + b`                 |

## Package Configuration

### Platform-IDE-Terminal (2.8.1)

```json
"platformio-ide-terminal":
  ansiColors:
    normal:
      black: "#003541"
      blue: "#268bd2"
      cyan: "#2aa198"
      green: "#859901"
      magenta: "#d33682"
      red: "#dc322f"
      white: "#eee8d5"
      yellow: "#b58901"
  core:
    scrollback: 10000
  iconColors:
    blue: "#0433ff"
  style:
    fontFamily: "Meslo LG M DZ for Powerline"
    fontSize: "16"
    theme: "solarized-dark"
  zBright:
    brightBlack: "#002833"
    brightBlue: "#839496"
    brightCyan: "#93a1a1"
    brightGreen: "#586e75"
    brightMagenta: "#6c6ec6"
    brightRed: "#cb4b16"
    brightWhite: "#fdf6e3"
    brightYellow: "#657b83"
  toggles:
    autoClose: true
    runInsertedText:false
```

## Trouble Shooting

> Turns out in my case, another package I installed stole that mapping. I hit CMD+. (CTRL+. on Windows) to launch the keyboard resolver and then hit CTRL+SHIFT+M and it showed another package as the one responding to the mapping and not the Markdown Package. I ended up uninstalling that other package, but I could have easily remapped that package to another key combo.

## Reference

-   [Awesome Atom](https://github.com/mehcode/awesome-atom)
-   [Atom Keyboard shortcuts](https://github.com/nwinkler/atom-keyboard-shortcuts)
-   [Atom Tips](https://www.sitepoint.com/12-favorite-atom-tips-and-shortcuts-to-improve-your-workflow/)

### CheatSheet

-   [Atom Editor Cheat Sheet (Bugsnag)](https://blog.bugsnag.com/atom-editor-cheat-sheet/)

### Themes

-   [The best Atom packages and themes](https://medium.com/@Dannypaton/the-best-packages-and-themes-for-atom-fee4860a7955)
-   [Shopify: Best Atom packages 2017](https://www.shopify.com/partners/blog/best-atom-packages-2017)
