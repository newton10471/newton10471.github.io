---
layout: post
category : lessons
title: Test code snippets
tagline: 
tags : [code, development]
---

Here's a simple test of code snippet formatting:

{% highlight ruby linenos %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}
