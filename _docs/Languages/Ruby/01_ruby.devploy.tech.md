---
title: "Ruby Deployment Tech"
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

$ sudo apt-get install -y build-essential sqlite3 git-core curl bison python-software-properties
$ sudo apt-get install -y libssl-dev libreadline-dev libyaml-dev libsqlite3-dev libxml2-dev libxslt1-dev
$ sudo apt-get install -y libcurl4-openssl-dev libffi-dev zlib1g-dev libgdbm-dev
$ wget https://cache.ruby-lang.org/pub/ruby/2.5/ruby-2.5.0.tar.gz
$ tar xvf ruby-2.5.0.tar.gz
$ cd ruby-2.5.0
$ ./configure
$ make -j 4
$ sudo make install

$ git clone https://github.com/rbenv/rbenv.git ~/.rbenv
$ cd ~/.rbenv && src/configure && make -C src
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
$ source ~/.bash_profile

# ruby-build
# As an rbenv plugin
$ mkdir -p "$(rbenv root)"/plugins
$ git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build

$ rbenv install --libxslt1
$ rbenv install 2.5.0

```

## Modern Web Development workflow

### Package Management

* Automation
* Organization
