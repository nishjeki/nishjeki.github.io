---
title: Xamarin.Forms to native Xamarin.iOS conversion
date: 2016-09-23 00:00:00 Z
categories:
- blog
tags:
- Xamarin Forms
- Xamarin native
- convert
layout: page
subheadline: 
teaser: Converting Xamarin.Forms to native Xamarin.iOS app using storyboard.  Requires
  some attention in overriding Window property in AppDelegate.
comments: true
---

## Steps:

1. Add storyboard and use native controls in your Forms.iOS project.

2. Update the info.plist to use this newly added storyboard as "Main Interface".

3. Modify the AppDelegate by extending UIApplicationDelegate and overriding Window Property as:

```cs
public partial class AppDelegate : UIApplicationDelegate
{
    public override UIWindow Window
    {
        get;
        set;
    }

    public override bool FinishedLaunching (UIApplication app, NSDictionary options)
    {
        return true;
    }
}
```

See in action here:
<br>
<iframe width="420" height="315" src="http://www.youtube.com/embed/-Q4VQ0i6fQ4" frameborder="0" allowfullscreen></iframe>
Why override Window property?
Check [this](http://nishjeki.github.io/blog/How-to-fix-black-screen-after-App-startup-in-Xamarin.iOS) out.
