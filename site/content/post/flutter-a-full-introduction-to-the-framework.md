---
title: "Flutter: a full introduction to the framework"
date: 2022-11-28T04:21:32.037Z
description: Flutter is a cross-platform software development framework that was
  presented by Google in 2015 and received its first release in May of 2017.
  Flutter nowadays has steadily grown and provided possibilities not only for
  iOS and Android mobile development but also for web and desktop applications
  as well. Let’s dive into the topic and try to understand why it is so popular
  nowadays.
image: https://uploads-ssl.webflow.com/5d359e0f47f4bbac7f9e3f50/5ef0924016b13a48ec71c173_madison-yocum-8OPCE5wJRMg-unsplash.jpg
---
## Table of Contents:

1. Dart: the language used by Flutter
2. Flutter Framework
3. Flutter Architecture
4. Conclusion

## Dart: t**he language used by Flutter**

Before we start deconstructing the Flutter framework, let’s dig into the language that was used to build it - the Dart. Dart is an object-oriented programming language that was first unveiled by Google in 2011. Since then Dart steadily evolved by releasing different features. Among others, it is worth mentioning the “dart2native” feature that allows compiling it for Windows, Linux, and macOS platforms as a desktop application. As of the writing this article, the desktop solution is not production-ready but the outlook seems promising. Aside from this, the Dart program can be composed into a self-contained executable file or compiled to JavaScript. The last one is especially notable because with compiling to JavaScript you can run Dart programs in every modern web-browser. But pay attention that the web solution is not production ready and currently in beta release. 

![](https://uploads-ssl.webflow.com/5d359e0f47f4bbac7f9e3f50/5ef0a6222587f65ed3c09cde_Yr-pWI4G_400x400.jpg)

Dart logo

In general, the Dart language is easy to study. Its syntax is pretty similar to Java, Swift, or Kotlin languages. Moreover, the Dart software development kit (SDK) is shipped with a stand-alone Dart Virtual Machine (VM) that allows you to build the code in a command-line interface (CLI) environment and if you are not familiar with CLI then you can play around with the Dart in DartPad. [DartPad](https://dartpad.dev/) is an online editor that provides access to Dart’s API and allows you to compile the Dart code. 

## Flutter **Framework**

As was previously mentioned, the Flutter framework was first unveiled by Google in 2015. Its code name was “Sky” and it ran on the Android operating system. The first stable release was delivered on the 4 of December 2018 and on May 6, 2020, the Dart SDK version 2.18 and Flutter version 1.17 were released delivering a build with Metal API integration. This has provided performance improvements to the iOS platform. 

The framework is written using C, C++, and Dart languages and uses Google’s Skia Graphics Engine for user interface rendering. This graphics engine is used for such known products as Google Chrome, Chrome OS, Chromium OS, Mozilla Firefox, Mozilla Thunderbird, Android, Firefox[ ](https://en.wikipedia.org/wiki/Firefox_OS)OS, and now the Flutter. 

![](https://uploads-ssl.webflow.com/5d359e0f47f4bbac7f9e3f50/5ef0a664ab7b6a925ddf8e64_flutter.png)

Flutter logo

Flutter runs using Dart virtual machine (VM) on Windows, Linux, and macOS operating systems. The Dart VM uses a just-in-time (JIT) code compilation which provides a development-time-saving feature such as hot-reloading. While the developer writes and debugs the mobile application, the JIT compilation injects new code into the running application. It provides a stateful hot-reload feature, where, in most cases source code changes can be immediately reflected in the running application without requiring a restart or any loss of state. This saves the developers’ a lot of time in the end. 

When it comes to releasing the application, the Dart VM uses the ahead-of-time (AOT) compilation which further converts Dart code into a native platform-dependent machine code making Flutter’s high performance on mobile devices possible. 

The Flutter framework was designed using some principles that should be described separately. These principles are “Everything’s a widget”, “Composition > Inheritance”, “Widget tree”. 

In Flutter almost everything is a widget and it is the basic building block of the application. Compared to other frameworks Flutter does not have separate controllers, views, or layouts. Almost every aspect of Flutter development is covered by a unified building block - the widget. A widget can be a unique button, style element, or a separate pop-up screen, etc.

The composition approach is better than inheritance. Often widgets are composed of other smaller widgets and that is the composition based approach. Using a Flutter API allows you to combine multiple widgets to elicit the exact behavior you need. 

![](https://uploads-ssl.webflow.com/5d359e0f47f4bbac7f9e3f50/5ef09355e0aae4af3454e106_bqEP6zM0XXJ2nJ_0awzo09EQpZsEQQsVHaA3oRM2bSKqmWOgbYz5Jtz_WW2L8yd_DfEFt39gjhM7Nrv8vZwZzO1Bp_aL_l37zcZRACefrBHwK2J19zLZvzYRRDPeVzB984Jw1gsF.jpeg)

Flutter System Overview, source: [flutter.dev](https://flutter.dev/docs/resources/technical-overview)

A widget tree concept is basically an implementation of nested widgets that represent user interface components. These widgets could be stateless or stateful and the difference between them is in keeping with the widget’s state. A useful feature that helps in managing the applications’ states. 

The most interesting thing about Flutter is the user interface components that were delivered with the latest releases. Google went by its own path and created two sets of widgets, Cupertino (iOS) and Material (Android). These sets of widgets are responsible for the user interface (UI) and include every component that you may need for Android and iOS development. These widgets are not connected with the native API of iOS or Android like in React Native but work as standalone Flutter components with appropriate rendering speed and animation. That is one of the key selling features of Flutter. Users will not be affected by poor user experience, because of it.