---
title: "Guide of Dart "
permalink: /docs/Database/Language/Dart/Flutter
excerpt: ""
last_modified_at: 2018-03-01T16:28:04+09:00
toc: false
---

# Flutter on Dart

## Installation

### Install Flutter SDK

```bash
# 0. Preinstallation Preparation (Mac)
$ sudo xcode-select --switch /Applications/Xcode-beta.app/Contents/Developer
$ sudo xcodebuild -license

$ sudo DevToolsSecurity -enable
$ pip install --upgrade pip && pip install six
$ brew install --HEAD libimobiledevice
$ brew install ideviceinstaller
$ brew install ios-deploy

# brew install cocoapods
$ sudo gem install cocoapods
$ pod setup

# 1. Install SDK
$ git clone -b beta https://github.com/flutter/flutter.git
$ export PATH=`pwd`/flutter/bin:$PATH
$ flutter config --no-analytics
$ flutter update
$ flutter doctor -v

# 2. Editor Setup
```

### Install Dart Command-line Tools

## Build Application

```bash
$ flutter create myapp
```

#### Reference

- [Cocoapods not work in macos
](https://stackoverflow.com/questions/44396215/cocoapods-not-working-in-macos-high-sierra)

## Introduction

> The key advantage of Flutter is that it provides reactive views without the need for JavaScript Bridge, hence improving the performance significantly. Another advantage is use of widgets. In Flutter, Everything’s a Widget.
> [Flutter handon ](https://blog.geekyants.com/flutter-hands-on-building-a-news-app-fe233027185f)

## Reference

### Flutter

-   [Official Document](https://flutter.io/docs/)
-   [Why use Dart](https://medium.com/@matthew.smith_66715/why-we-chose-flutter-and-how-its-changed-our-company-for-the-better-271ddd25da60)
-   [Why Flutter use Dart](https://hackernoon.com/why-flutter-uses-dart-dd635a054ebf)
-   [Why Dart not use OEM Widgets](https://medium.com/flutter-io/why-flutter-doesnt-use-oem-widgets-94746e812510)
-   [Revolution about Flutter](https://hackernoon.com/whats-revolutionary-about-flutter-946915b09514)

### Flutter Examples

- [FreecodeCamp: How to build ad cryptocurrency price List](https://medium.freecodecamp.org/how-to-build-a-cryptocurrency-price-list-app-using-flutter-sdk-1c75998e1a58)
