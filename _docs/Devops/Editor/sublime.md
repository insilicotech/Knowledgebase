---
title: "Sublime Text 3"
permalink: /docs/Devops/Editor/sublime-text3/
excerpt: "Sublime Text 3 "
last_modified_at: 2018-03-10T16:28:04-05:00
toc: false
---


## Themes

* Boxy
* Predawn

## Packages

* Origami

* Emmet
* ColorSublime

* ConvertToUTF8

* Markdown Preview
* LiveReload

## Installation

```powershell
PS> $reg = "HKCU:\Software\Microsoft\Windows\CurrentVersion\Internet Settings"

PS> netsh winhttp set proxy proxy-server="http=172.16.1.1:80;https=172.16.1.1:80" bypass-list="192.168.103.*;157.112.176.24;192.30.255.113;192.30.255.112;104.25.15.31;<local>" | Out-Null

```

```bash
git config --global user.email "ist@insilicotech.co.jp"
git config --global user.name "insilicotech"

git config --global http.proxy http://172.16.1.1:80
git config --global https.proxy http://172.16.1.1:80
git config --global http.sslVerify false

git config --global --unset https.proxy
git config --global --unset http.proxy

git clone https://github.com/insilicotech/Knowledgebase.git

git -c http.proxy= clone https://github.com/insilicotech/Knowledgebase.git
```

### Install node.js via Chocolatey

```bash
$ choco config set proxy http://172.16.1.1:80
$ choco config set proxyBypassOnLocal true 
$ nvm proxy http://172.16.1.1:80
$ nvm list avaliable
$ nvm install latest 32
$ nvm list
$ nvm use 9.8.0 32 
$ node -v; npm -v
$ npm -g config set http-proxy http://172.16.1.1:80
$ npm -g config set https-proxy http://172.16.1.1:80

$ choco install ruby
$ refreshenv
$ ruby -v
$ set http_proxy=http://172.16.1.1:80
$ set https_proxy=http://172.16.1.1:80
$ gem install bundler -p http://172.16.1.1:80

$ choco install googlechrome

set http_proxy=172.16.1.1:80
set https_proxy=172.16.1.1:80
```

Choco Download Directory
`C:\Users\Administrator\AppData\Local\Temp\chocolatey`

## Keyboard Shortcut


| Open new pane at right |`ctrl + K, ctl ->`  |


## Reference

* [The Best 10 Sublime Text3 Themes of 2017](https://scotch.io/@Viclotana/the-10-best-sublime-text-3-themes-of-2017)
* [Various Proxy Setting](http://dac01.sakura.ne.jp/howto/security/proxy_settings.html)


