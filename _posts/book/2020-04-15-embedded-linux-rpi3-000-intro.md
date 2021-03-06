---
title : Embedded Linux with Raspberry Pi 3 Model B
layout : post
category : book
date: 2020-04-13 22:14:31 +5:30
comments: true
google_adsense: true
excerpt : A series of articles about Embedded Linux - Integration of bootloader, kernel, system libraries and the third party applications -  using Raspberry Pi Model B.
kerwords : Embedded Linux book for Raspberry Pi Model B, Embedded Linux tutorial, Embedded Linux development, Embedded Linux tutorial, Embedded Linux with Raspberry Pi Model B, Device driver development on Raspberry Pi Model B, Embedded Linux OS, Learning device drivers on Rapsberry Pi Model B, Develop Linux from scratch on Raspberry Pi Model B
image : /assets/img/rpi3b-elinux-intro.png
toc : true
---
## Introduction

Embedded Linux development for any *single board computer* (SBC) or *embedded development board* typically involves integration of -
 - Kernel
 - Boot loader
 - System libraries and
 - Third party applications (if needed).

Before chosing to develop the Embedded Linux system, make sure there is *Linux* and open source boot loader like *U-boot* support for SoC.

{% include image.html url="rpi3b-elinux-intro.png" description="Embedded Linux with Rapsberry Pi 3 Model B" %}
## Requirements
The following hardware required to develop an Embedde Linux system.

 - Raspberry Pi Model B
 - A laptop / desktop with Ubuntu Linux
 - An HDMI cable
 - A HDMI capable monitor or TV
 - An USB keybord
 - A good broadband connection

## Why Raspberry Pi
Raspberry Pi has extensive Linux and U-boot support. There are official Linux distributions from [Debian](https://www.raspbian.org/), [Ubuntu](https://ubuntu.com/download/raspberry-pi) and [others](https://www.raspberrypi.org/downloads/). Learning and developing is easy when there is quite a large community of developers and tinkerers to get help.

## Learning path
Consider following list of articles as a *table of contents* or the *overview of the learning path*.
{% assign cat = "rpi3b-elinux" %}
<ul class="list-none">
{% for category in site.categories %}
{% if category.first == cat %}
{% assign sorted = (category[1] | sort: 'url') %}
{% for posts in sorted %}
<li><a class="post-link" href="{{ posts.url }}">{{ posts.title | remove : "for Raspberry Pi 3 Model B" | remove : "of Raspberry Pi 3 Model B" | remove : "with Raspberry Pi 3 Model B"}}</a></li>
{% endfor %}
{% endif %}
{% endfor %}
</ul>


**More articles coming**....
