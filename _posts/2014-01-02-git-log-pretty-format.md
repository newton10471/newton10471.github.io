---
layout: post
category : lessons
title: git log with pretty formatting
tagline: "Customize the heck out of git log output"
tags : [intro, beginner, git]
---

You can customize git log output with a fair amount of granularity by using the "--pretty=format:" option, as in the following: 

{% highlight bash %}
  user@ws ~/projects/ruby(master)$ git log --pretty=format:"%h %cd %ae  %s" --date=short --after="2013-12-04"
  1abcdef 2013-12-10 user1@ws.net  fix issue 1
  2ghijkl 2013-12-09 user2@ws.net  fix issue 2
  3333333 2013-12-09 user2@ws.net  fix issue 3
  user@ws ~/projects/ruby(master)$
{% endhighlight %}

Details are at [http://git-scm.com/docs/git-log](http://git-scm.com/docs/git-log), under the "format:\<string\>" bullet.
