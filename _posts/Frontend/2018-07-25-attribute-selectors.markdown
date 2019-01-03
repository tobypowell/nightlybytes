---
layout: post
title: "Attribute Selectors in both css and jQuery"
date: '25 July 2018'
body-class: 'inner-page'
category: 'frontend'
description: 'A selection of useful and powerful attribute selectors used in css and jQuery to make selecting and working with dom elements much easier!'
main-image: 'https://images.unsplash.com/photo-1472437774355-71ab6752b434?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=dd4d735954f33290fbf984e4eb7abe32&auto=format&fit=crop&w=967&q=80'
---

Attribute selectors are easily recognisable as they are wrapped in square brackets: input[type='text']

#### ^= the begining of a string.
{% highlight css %}
    a[href^='http://']
{% endhighlight %}
The '^' (caret) character is used to specify a match at
So the above selector will find all links thats href attribute begins with 'http://'

### !=
The '!' character specifies everything except that preceeds the 'not equal to' character:
{% highlight css %}
    a[href!='http://jquery.com]
{% endhighlight %}
The above selector selects all the links **except** the links with the href attribute of 'http://jquery.com'

### $=
The $ character specify atrributes that **end** with whatever preceeds the dollar sign:
{% highlight css %}
    a[href$='.pdf']
{% endhighlight %}

### *=
The * selects all the elements
{% highlight css %}
    a[href*='jquery.com']
{% endhighlight %}

### |=
The |= 'contains' selector selects all the elements that contain the string specified
{% highlight css %}
    div[class|='main']
{% endhighlight %}