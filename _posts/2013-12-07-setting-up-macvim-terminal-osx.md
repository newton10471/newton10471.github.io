---
layout: post
category : lessons
title: Setting up terminal MacVim on Mac OS X
tagline: "Always had trouble getting this working before"
tags : [vim, development]
---

I struggled to get this to work before but finally found a solution to having 'vim' invoke terminal MacVim on Mac OS X instead of the default (outdated and compiled with minimal config) vim that comes with it. Based on [this post](http://apple.stackexchange.com/questions/14299/replaced-usr-bin-vim-now-i-get-error-messages), it looks like you can do the following to make this work:

1. make sure the 'mvim' utility included in the MacVim install works from your default command line shell
2. set the this alias in your .bash\_profile or .bash\_login startup file: 

{% highlight bash %}
  alias vim='/usr/local/bin/mvim -v'
{% endhighlight %}

I have this in my own setup now and it works great.
