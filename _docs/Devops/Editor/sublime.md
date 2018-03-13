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

* Emmet
* ColorSublime
* ConvertToUTF8

## Installation

```powershell
PS> $reg = "HKCU:\Software\Microsoft\Windows\CurrentVersion\Internet Settings"

PS> netsh winhttp set proxy proxy-server="http=172.16.1.1:80;https=172.16.1.1:80" bypass-list="192.168.103.*;192.30.255.113;192.30.255.112;104.25.15.31" | Out-Null

```

```bash
git config --global http.proxy http://172.16.1.1:80
git config --global https.proxy http://172.16.1.1:80
git config --global http.sslVerify false

git config --global --unset https.proxy
git config --global --unset http.proxy

git clone https://github.com/insilicotech/Knowledgebase.git

git -c http.proxy= clone https://github.com/insilicotech/Knowledgebase.git
```

## Reference

* [The Best 10 Sublime Text3 Themes of 2017](https://scotch.io/@Viclotana/the-10-best-sublime-text-3-themes-of-2017)
