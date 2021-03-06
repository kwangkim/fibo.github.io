---
title: Livereload with grunt
tags:
  - Node
description: >
    Instructions to configure Grunt to interact with a Livereload server.
---

## What you get

After changing your html, css and js files, you don't need to refresh your browser to see changes.

<div class="alert alert-info">Your page will <strong>magically</strong> change, as you save your files!</div>

## Requirements

Create a *package.json*

```bash
$ cd /path/to/your/working/folder/
$ npm init
```

Install *grunt-cli* globally (only once).

```bash
$ npm uninstall -g grunt-cli
$ npm install -g grunt-cli
```

Install *grunt* and other packages

```bash
$ npm install --save-dev grunt
$ npm install --save-dev grunt-contrib-connect
$ npm install --save-dev grunt-contrib-watch
$ npm install --save-dev grunt-open
```

## Configuration

I suppose there is at least an *index.html* and some JavaScript file under *js/* folder.
I like to use [coffee-script][3] to edit configuration, i.e. I use a *Gruntfile.coffee*

Here it is a working configuration

{% gist fibo/7054215 %}

Now, if you launch

```bash
$ grunt
```

<div class="alert alert-success">Your browser will open, and the window will change <strong>as soon as</strong> you modify your files.</div>

## See also

* [Node ecosystem](http://g14n.info/2014/01/node-ecosystem)
* [Install Node.js without sudo](http://g14n.info/2013/01/install-nodejs-without-sudo)
* [Create an npm package](http://g14n.info/2014/01/create-npm-package)
* [Badges everywhere](http://g14n.info/2014/01/badges-everywhere)
* [NodeICO badges](http://g14n.info/2013/12/nodeico-badges)
* [Node class template](http:/g14n.info/2014/01/node-class-template)


  [1]: http://gruntjs.com/
  [2]: http://livereload.com/
  [3]: http://coffeescript.org/

