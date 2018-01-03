# Mattress Firm - Landing Pages
## Project Setup
* You will need a virtual host / server. Currently we are using [MAMP / MAMP Pro](https://www.mamp.info/en/mamp-pro/).
    * *Currently using PHP for templating.*
* In MAMP setup a new host as **MattressFirm** and point it to the project root directory. 
* Install [Node.js](https://nodejs.org/en/), [Sass](http://sass-lang.com/) and [Git](https://git-scm.com/). 
    * *If you're a Windows user you'll also need to install Ruby.*
* Install [Gulp](https://gulpjs.com/) using `npm install -g gulp`. 
* Install dev dependencies with `npm install`.
* Navigate to [MattressFirm/app](http://mattresfirm/) or [localhost:3000](http://localhost:3000/).
## Demandware Deployment Process
* **In Sandbox** Create new content asset.
* Lock the content asset.
* Copy markup to new or existing content asset.
* Remove `<?php include 'header.php'; ?>` and `<?php include 'footer.php'; ?>`.
* Make sure custom styles and scripts are included:
    * `<link rel="stylesheet" href="css/cl-style.min.css?$staticlink$">`
    * `<script type='text/javascript' src='//ajax.googleapis.com/ajax/libs/jquery/2.1.0/jquery.min.js?ver=2.1.0'></script>`
    * `<script type='text/javascript' src='js/cl-scripts.min.js?$staticlink$'></script>`
* Make sure images have the following:
    * Same path on your local environment and Demandware environment.
        * *So you don't have to update the link when copying.* 
    * All image paths should end with `?$staticlink$`.
* Upload Images.
* Copy `styles.min.css` from `app/css`, rename to `cl-styles.min.css` and upload to Demandware.
    * *Only if css was been updated.*
* Copy `scripts.min.js` from `app/js`, rename to `cl-scripts.min.css` and upload to Demandware.
    * *Only if JS was been updated.* 
* **QA and with client approval repeat process to Staging.** 
## Built on FastShell
[![Build Status](https://travis-ci.org/HosseinKarami/fastshell.png?branch=master)](https://travis-ci.org/HosseinKarami/fastshell)

inspired by [FireShell](http://getfireshell.com)
Fiercely quick front-end boilerplate and workflows.

The opinionated FastShell framework. Built for the modern developer. For teams and the individual, encouraging a better workflow. JavaScript task running, build processes, autominification and file concatenation, wrapped with an enhanced HTML5 boilerplated framework.

* Source: [github.com/HosseinKarami/fastshell](http://github.com/HosseinKarami/fastshell)
* Documentation: [DOCS.md](https://github.com/HosseinKarami/fastshell/blob/master/DOCS.md)
* HomePage: [Fastshell](https://HosseinKarami.github.io/fastshell)
### License
##### The MIT License (MIT)
Copyright (c) FastShell
Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
