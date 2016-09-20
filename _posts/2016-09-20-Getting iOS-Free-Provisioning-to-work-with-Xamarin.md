---
disqus: true
layout: post
title: Getting free provisioning to work for Xamarin
description: Fixing "No installed provisioning profiles match the installed iOS signing identities" error.  Its the bundle identifier causing trouble.
---

While using a device such as iPhone or iPad for debugging with Xamarin Studio it gives error as:

>"No installed provisioning profiles match the installed iOS signing identities".

This is because Xamarin Studio project wizard creates bundle identifier as *"com.nishjeki.myapp"*

Whereas the xcode project wizard creates bundle identifier as *"com.nishjeki.myApp"*

The *myApp* with a capital *'A'* causes the problem.

There are similar small issues which comes while using Free Provisioning, I've tried to capture them in a video.
See in action here:

<iframe width="420" height="315" src="http://www.youtube.com/embed/S9lNmnyACpY" frameborder="0" allowfullscreen></iframe>

