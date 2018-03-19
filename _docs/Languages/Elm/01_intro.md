---
title: "Elm Guide"
permalink: /docs/Language/Elm/guide/
excerpt: ""
last_modified_at: 2018-03-12T16:28:04-05:00
toc: false
---

# Elm Guide Book

## Installation

```bash
$ npm install -g elm
$ npm install -g elm-format elm-graphql
```

### Editor Setting

```bash
$ atom install elm-format
```

### Elm Commands

-   elm-repl
-   elm-make
-   elm-package
-   elm-reactor

## Language Basics

### Partial Function Application

**|>** Forward function application operator

```elm
speed distance time =
  distance / time

time startTime endTime =
  endTime - startTime

escapeEarth velocity speed =
  if velocity > 11.186 then
    "Godspeed"
  else if speed == 7.67 then
    "Stay in orbit"
  else
    "Come back"

main =
  time 2 3
    |> speed 7.67
    |> escapeEarth 11
    |> Html.text
```

| Library | Creator        |
| ------- | -------------- |
| Elm     | Evan Czaplicki |
| Redux   | Dan Abramov    |

### Let Expression in Function

```elm
escapeEarth velocity speed =
  let
    escapeVelocityInKmPerSec =
      11.186
    orbitalSpeedInKmPerSec =
      7.67
  in
    if velocity > escapeVelocityInKmPerSec then
      "Godspeed"
    else if speed == orbitalSpeedInKmPerSec then
      "Stay in orbit"
    else
      "Come back"
```

### Filter

```elm
> String.filter (\char -> char /= '-') "222-11-5555"
"222115555"
```

![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

## Reference

### TLDR

-   Pure functions -> Native
-   Immutable data structures -> Immutable.js
-   Higher-order functions -> Native
-   Currying -> Ramda.js
-   Static type checking -> Flow (Not JavaScript)
-   No concept of Null -> folktale/data.maybe
-   Reactivity -> Rx.js
-   The Elm Architecture -> Redux
-   Declarative UI -> React.js


-   Elm or React/Relay
-   Phoenix
-   GraphQL
-   Rethinkdb (will write a blogpost on this choice aswell)

### Guild & Tutorial

-   [Official Guild](https://guide.elm-lang.org/)
-   [Online Guide |> Beginning Elm](http://elmprogramming.com/)
-   [Playground: Try Elm online](http://elm-lang.org/try)
-   [Ellie](https://ellie-app.com/new)
-   [FrontendMaster ELM Online Course](https://frontendmasters.com/courses/elm/)
-   [Elm Architecture Tutorial ](https://github.com/pawanpoudel/elm-architecture-tutorial)

### Use Cases & Success Stories

-   [Move fast and don’t break things. Running a startup on Elm](https://medium.com/the-ahead-story/move-fast-and-dont-break-things-running-a-startup-on-elm-b5491082fe8b)
-   [Learning FP the hard way: Experiences on the Elm language](https://gist.github.com/ohanhi/0d3d83cf3f0d7bbea9db)

### MISC

-   [Mark Sheet](https://marksheet.io/)
