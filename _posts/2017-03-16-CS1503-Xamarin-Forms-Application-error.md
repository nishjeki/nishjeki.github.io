---
title: CS1503 Xamarin.Forms.Application error
date: 2017-03-16 00:00:00 Z
categories:
- blog
tags:
- CS1503
- Xamarin.Forms.Application
- UWP
- Xamarin Forms
comments: true
subheadline: 
teaser: While adding a UWP app an error might be encountered as CS1503:Cannot convert
  from [type] to type Xamarin.Forms.Application for UWP'. Just make sure to use the
  correct App class.
layout: page
---

I encountered this error when I added a new UWP project to my existing Xamarin Forms solution and tried building it. 

My solution was created using Xamarin Studio on Mac some time ago.  Xamarin Studio created the App class in a Forms.cs file in the portable Xamarin.Forms project. This confused me that App class even exists.
When I tried to create a UWP project using Visual Studio on Windows I came across this error.

I was following the Xamarin Forms [help](https://developer.xamarin.com/guides/xamarin-forms/platform-features/windows/installation/universal/) site to create a UWP app where it is not mentioned.
The solution is simple enough, just use the App object from the portable library instead of the UWP library in LoadApplication() method.

This issue will not arise when the solution is created using latest Visual Studio.

<br>
See in action here:
<br>
<iframe width="420" height="315" src="http://www.youtube.com/embed/jLCUfolFQF0" frameborder="0" allowfullscreen></iframe>