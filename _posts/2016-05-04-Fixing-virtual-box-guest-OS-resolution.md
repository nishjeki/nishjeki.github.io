---
title: Fixing virtual box guest OS resolution
date: 2016-05-04 00:00:00 Z
categories:
- blog
tags:
- virtual box
- resolution
- mac os
layout: page
subheadline: 
teaser: Fixing resolution issue with Virtual box on Mac OS as host and Windows 10
  or Debian Linux as guest OS.
comments: true
---

Just installing a Virtual Box application and installing guest Operating systems won't provide required resolutions.

This is true in case of both Windows OS and Linux OS as guest and Mac OS as host.

The guest OS might not scale to the host resolution and might need scrolling and look like this:

<img src="{{site.url}}/images/virtualbox-resolution-issue-win10-guest.png"/>
(Visible scroll bars)


It needs installing virtualbox guest additions inside the guest operating systems.

For [Debian Linux](http://virtualboxes.org/doc/installing-guest-additions-on-debian/)

For [Windows 10](https://www.virtualbox.org/manual/ch04.html#additions-windows)

It should be similar for any other guest operating systems if resolution issue exists.