---
layout: post
title: "Sponge of pipes "
description: "A command that let you pipe from one file to itself."
category: "commands"
tags: [commands, pipe]
---
{% include JB/setup %}

{% highlight bash startinline %}
cmd1 $file | sponge﻿ $file
{% endhighlight %}


With `sponge` at the end you can manipulate the file before and write to itself. But be careful if the commands before `sponge` exit for some reason the file might be lost and you produce a empty file. 