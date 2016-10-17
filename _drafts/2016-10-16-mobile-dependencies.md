---
layout: post
title: Mobile Dependency Management
cover: ios-notification-centre.jpg
---

If you’re working on native mobile app. development it’s practically a guarantee that you’ll  work on project that requires third party libraries. e.g. using Facebook’s SDK to support Login With Facebook in your app. Once a project depends on a third party library, we can call that library a project dependency.

Dependency management is a common task for any development environment, it’s not unique to mobile development and yet on mobile it can feel very broken, unfortunately more broken when developing for iOS than Android.

With mobile development there are a lot of fast moving parts when it comes to actually collecting all the resources that make up your project and assembling them into an app that can be installed on a device. This process is known as building the app. Both iOS and Android come with fairly robust build systems.

So, why does Android’s dependency management suck less than that of iOS?

Here is the one line of code I need to add to my Android project’s Gradle configuration to enable me to work with Facebook’s Login Toolkit:

compile 'com.facebook.android:facebook-android-sdk:4.+'

Achieving the equivalent setup on Xcode for iOS is not as simple. There are some third party dependency managers that attempt to provide this functionality for Xcode but they’re not officially supported nor are they anywhere as easy to use.

However I’ll note that iOS' more complicated dependency management is the exception and not the rule. Typically Apple has gone out of its way to make iOS development as pleasant as possible. Their recent enhancements to interface builder and the most recent revision of the Swift programming language are just two examples of their ongoing efforts to keep iOS development as streamlined as possible. Logic dictates that someone at Apple is already cracking away at this problem.
