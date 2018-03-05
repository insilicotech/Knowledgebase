---
title: "Introduction of Vue"
permalink: /docs/FontEndDevelopment/Ruby/ruby-deploy-tech/
excerpt: "How to quickly install and setup Minimal Mistakes for use with GitHub Pages."
last_modified_at: 2018-03-05T16:28:04-05:00
toc: false
---

## Setup Vagrant/Vitual-box Environment

``` bash
$ vagrant init ubuntu/trusty64
$ vagrant up
$ vagrant ssh

$ sudo apt-get update
$ sudo apt-get install -y build-essential git-core python-software-properties

$ curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
$ sudo apt-get install -y nodejs

$ sudo apt-get install ruby-full

$ wget https://cache.ruby-lang.org/pub/ruby/2.5/ruby-2.5.0.tar.gz
$ tar xvf ruby-2.5.0.tar.gz
$ cd ruby-2.5.0
$ ./configure
$ make -j 4
$ sudo make install
```
