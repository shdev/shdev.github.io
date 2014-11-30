---
layout: post
title: "Network bridge"
description: "Build a bridge over 2 network devices"
category: commands
tags: [command, darwin, network, bridge, sudo]
---
{% include JB/setup %}

{% highlight bash startinline %}
sudo ifconfig bridge0 create
sudo ifconfig bridge0 addm en0 addm en1
sudo ifconfig bridge0 up
{% endhighlight %}