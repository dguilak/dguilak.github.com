---
layout: post
title: "Installing OpenCV 2 in Mac OS X Lion"
description: "Gotchas in installing OpenCV 2 for Python 2.7 use in Mac OS X Lion using MacPorts"
category: 
tags: [mac, mac os x, os x, opencv]
---
{% include JB/setup %}

For our senior capstone project, [Josef Lange](http://josefdlange.com/) and I are working on a tablet-enabled mathematical expression parser we're calling [Expresso](http://github.com/expresso-math/). Since it's really just a proof of concept at this point, we're going to be using some basic OpenCV machine learning functionality to do symbol recognition. Apparently, it can be a bit of a pain to install OpenCV for Python use, so here's what ended up working for me:

{::options parse_block_html="true" /}
I use the [MacPorts](http://www.macports.org/) package manager, so install that if you haven't already. I believe you'll need XCode installed as well.

<div class="p">
First update MacPorts with
</div>

~~~
sudo port selfupdate
~~~

Then make sure you [accept the Apple license](http://trac.macports.org/ticket/35337) for XCode, otherwise gnuplot will fail to build later on and cause many headaches:

~~~
sudo xcodebuild -license
~~~

Finally you can install OpenCV with Python 2.7 functionality using

~~~
sudo port install opencv +python27
~~~

per the instructions located on the [OpenCV wiki](http://opencv.willowgarage.com/wiki/Mac_OS_X_OpenCV_Port).
