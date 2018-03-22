---
title: "VSCode"
permalink: /docs/Devops/Editor/vscode/
excerpt: "Visual Studio Code Editor"
last_modified_at: 2018-03-10T16:28:04-05:00
toc: false
---

```powershell
PS> atrib -H \ProgramData
PS> atrib -H \Users\Adminstrator\AppData
```

## Construction

### Package Manager

- Chocolatey

### Source Management

- git

### Browser

- Chrome

### Lanagues

- NodeJS
- Ruby
- Python2
- Elm
- Haskell
- Go
- Rust

### Editor

- Atom
- Sublime Text 3
- VSCode
- Bracket

### Terminal

- cmder
- Butterfly


Ruby | C:\tools\ruby25
Python2 | C:\Python27

```powershell
PS>  python -m pip install --upgrade pip
```

## Installation

```powershell
PS> choco install cabal
PS> choco install ghc
```

In your Cmder folder, create a file labeled `atom.bat`
```batch
@echo off
SET CMDER_ROOT=C:\tools\cmder
"%CMDER_ROOT%\vendor\init.bat"
```

3. Adjust the Package Settings:

Shell Override:
C:\Windows\System32\cmd.exe

Auto Run Command:
"C:\tools\cmder\atom.bat"

Setting PATH

`C:\IST\Bin\Atom`
`C:\IST\Bin\Atom\resources\app\apm\bin`

### atom
```bash

apm config set strict-ssl false
apm config set http-proxy http://172.16.1.1:80
apm config set https-proxy http://172.16.1.1:80

apm install platformio-ide-terminal

```


## Reference

- [TheBar: Atom + Cmder](http://thebar.cc/atom-editor-cmder/)
