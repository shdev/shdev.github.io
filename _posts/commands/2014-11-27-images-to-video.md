---
layout: post
title: "Images to video"
description: ""
category: "commands"
tags: [command, ffmpeg, image, video]
---
{% include JB/setup %}


{% highlight bash startinline %}
ffmpeg -f image2 -i %04d.jpg -qscale:v 0.1 video.mpg
{% endhighlight %}


with `-r 24` you should adjust a framerate of images per second.