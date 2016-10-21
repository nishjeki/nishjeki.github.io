---
layout: page
title:  "How to fix black screen after App startup in Xamarin.iOS"
subheadline:
teaser: "While using storyboard in Xamarin.iOS sometimes permanent black screen appears. A simple fix is to override the Window property in AppDelegate class."
categories:
    - blog
tags:
    - black screen
    - Xamarin.iOS
    - AppDelegate
comments: true
---

Black screen appears after App startup while using story board as:

<img src="{{site.url}}/images/blackscreen-after-app_start-in-storyboard.png"/>

The Application output in Xamarin Studio clearly states:

> The app delegate must implement the window property if it wants to use a main storyboard file.

Hence to fix : Go to your AppDelegate class and override the Window property as:

```cs
public partial class AppDelegate : UIApplicationDelegate
{
	public override UIWindow Window
	{
		get;
		set;
	}
```

And that’s it!

See in action:

<iframe width="420" height="315" src="http://www.youtube.com/embed/UVkbkXCm1vU" frameborder="0" allowfullscreen></iframe>

