---
layout: post
title:  "Control sound via the commandline"
date:   2016-08-28 22:02:03 +0200
categories: linux commandline sound
---

### Control sound volume via commandline

Problem: Between doing various configuration changes and unplugging my speakers, Youtube didn't play sound anymore!

Solution: On windows you'd click on that speaker tray icon; on Ubuntu/i3 this worked:

{% highlight ruby %}
amixer -D pulse sset Master unmute
amixer -D pulse sset Master 100%
{% endhighlight %}

to mute:
{% highlight ruby %}
amixer -D pulse sset Master mute
{% endhighlight %}
