wxWidgets Website
=================

The wxWidgets website is built using [Jekyll][jekyll], using [Node.js][node]
and [Grunt][grunt] to compile all static assets including the
[Bootstrap][bootstrap] library the site is built on along with the
[Font Awesome][fa] icon set using [LESS][less] stylesheets. Most of the content
on the website is written using [Markdown][markdown], making it extremely easy
to write and maintain.

[jekyll]: http://jekyllrb.com/
[node]: http://nodejs.org/
[grunt]: http://gruntjs.com/
[bootstrap]: http://getbootstrap.com/
[fa]: http://fontawesome.io/
[less]: http://www.lesscss.org/
[markdown]: http://daringfireball.net/projects/markdown/

## Quick-start Guide

We've prepared a Vagrant configuration that can automatically install and
configure all dependencies listed above. So it's a bit more to download, but is
the quickest and most reliable way to dive right in if you aren't already
familiar with Jekyll, Node.js, and Grunt. Simply download and install both
[VirtualBox][vb] and [Vagrant][vagrant], and run the following from a command
prompt in this checkout:

    $ vagrant up

This will take a while to complete the first time, just be patient. After your
Vagrant box is up and running, you can SSH in by running:

    $ vagrant ssh

This checkout will be shared with this virtual machine at `/vagrant`, so you
can go there now and run `grunt` to compile all assets, and run `jekyll` to
start up the built-in webserver that will automatically re-generate all pages
any time it's corresponding file is changed here.

    $ cd /vagrant
    $ npm install
    $ grunt
    $ jekyll serve --watch

Note that you only need to run `npm install` once per new checkout. Now you can
edit content at will and see the immediate feedback by pulling up the website
running inside of your Vagrant box: <http://localhost:4000/>

[vb]: https://www.virtualbox.org/wiki/Downloads
[vagrant]: http://www.vagrantup.com/downloads.html

## Minimal Setup for Content Editing Only

If you only want to modify some page contents and are not going to touch any
CSS or JavaScript code, you can avoid installing [Grunt][] as it is only
really needed to produce the minified CSS and JavaScript files which can be
retrieved from the main site:

    $ curl http://www.wxwidgets.org/assets/css/global.min.css > assets/css/global.min.css
    $ curl http://www.wxwidgets.org/assets/js/global.min.js > assets/js/global.min.js

Then you only have to install [Jekyll][] and run it in order to preview your
changes locally before pushing them out.
