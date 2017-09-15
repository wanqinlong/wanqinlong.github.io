---
title: 《物联网 (IoT)  | Android Things Developer Preview 5 》
date: 2017-9-15 13:12:38
categories: #法律法规 #文章分类目录 可以省略  <!--more-->
- Google
- 物联网 (IoT)
tags: #文章标签 可以省略
- 物联网 (IoT)
---
2017年8月23日星期三

﻿发布人：IoT 开发技术推广工程师 [Wayne Piekarski](https://google.com/+WaynePiekarski) 

我们宣布推出 [Android Things](https://developer.android.google.cn/things/index.html) 的 Developer Preview 5 (DP5) 版本，该版本包含基于未来 Android O 版本的重要变更。Android Things 是 Google 推出的平台，旨在帮助 Android 开发者打造物联网 (IoT) 设备，并从原型开发无缝扩展到量产。
# Android O #
对于手机和平板电脑，Android O 目前正处于 [Developer Preview](https://android-developers.googleblog.com/2017/07/developer-preview-4-now-available.html) 阶段，而 DP5 则恰恰基于这一即将发布的版本（之前的版本基于 Android N）。这意味着，您未来的 Android Things 应用应针对 API 26，方可在该平台上正确使用我们的支持库。
# 硬件变更 #
现在，DP5 新增了对全新 [NXP SprIoT i.MX6UL](https://developer.android.google.cn/things/hardware/imx6ul.html) 设计的支持，在我们的开发者套件[文档](https://developer.android.google.cn/things/hardware/developer-kits.html)中列出了这一变更。随着 Intel 停止 [Edison](https://software.intel.com/en-us/iot/hardware/edison) 和 [Joule](https://software.intel.com/en-us/iot/hardware/joule) 硬件设计，这些平台即将转入旧设备支持阶段。它们不会继续收到最新的平台更新，但开发者仍可从 Android Things 管理中心继续获取 DP4.1 系统映像。 

Android Things 的一个重要目标是：帮助开发者从原型开发无缝扩展到量产。当我们结束 Developer Preview 时，我们将会在以仅原型开发为目标的硬件平台和可扩展到量产的硬件参考设计之间进行差异化。可量产的硬件将满足 Google 的安全要求并享有硅半导体制造商的长期支持。稍后，我们还会分享更多内容。

- NXP SprIoT i.MX6UL

![](https://i.imgur.com/EalbvxB.png)

<!--more-->

- Edison

![](https://i.imgur.com/zeJq8Lv.png)

- Joule

![](https://i.imgur.com/JeDxth1.png)

# 改进 #
随着我们开始迁移到 Android O 代码库，Android 中提供了一些新的 API 功能，还有一些专门针对 Android Things 的功能。对于使用 UserDriver API 的开发者来说，您将需要在 AndroidManifest.xml 中添加新的权限。[文档](https://developers.android.com/things/sdk/drivers/index.html)中包含有关每种类型的驱动程序所需的权限详情。DP5 现在还支持在 Raspberry Pi 3 平台上运行 OpenGL ES 2.0 和 WebView，这是开发者社区呼声甚高的一项功能。我们还针对 Raspberry Pi 3 实现了[动态引脚多路复用](https://developer.android.google.cn/things/hardware/raspberrypi-mode-matrix.html)功能，引脚在运行时根据所要使用的功能进行配置。
# Android Studio #
现在，可直接在 Android Studio 中获取 Android Things 示例，以进行浏览和导入。现在，只需进入 File、New、Import Samples 并搜索 Things，即可查看提供的所有示例。我们提供丰富多样的示例，展示了如何与按钮、传感器、LED 和显示屏交互以及如何实现 Google 智能助理和 TensorFlow。
# Android Things 管理中心 #
我们最近[启动](https://android-developers.googleblog.com/2017/06/android-things-console-developer-preview.html)了 [Android Things 管理中心](https://partner.android.com/things/console)，其能够支持对 Android Things 设备的无线更新 (OTA)。我们最近对该管理中心做出了大量用户体验方面的改进，以改善易用性和功能。DP5 现已可在 Android Things 管理中心内部获取，但未经您的干预，DP5 更新不会自动推送到设备。您需要针对 DP5 更新您的应用，然后创建一个新更新并通过管理中心自行推送更新。
# 反馈 #
在将 Android Things 更新到 Android O 时，我们对该平台做出了一些重要变更。请提[交错误报告](https://code.google.com/p/android/issues/entry?template=Android%20Things%20bug%20report)和[功能请求](https://code.google.com/p/android/issues/entry?template=Android%20Things%20feature%20request)，继续向我们发送您的反馈，并欢迎在 [Stack Overflow](https://stackoverflow.com/questions/tagged/android-things) 上提出任何问题。要开始使用 DP5，请使用 [Android Things 管理中心](https://partner.android.com/things/console)下载系统映像并更新现有设备。[版本说明](https://developer.android.google.cn/things/preview/releases.html)中提供了有关这些变更的更多信息。您也可以在 Google+ 上加入 Google 的 IoT 开发者社群，这是一个非常有用的资源，在这里，您可以了解最新消息并讨论想法。此外，我们还建立了新的 [hackster.io 社群](https://www.hackster.io/google)，在这里，每个人都可以分享他们创建的精彩项目！ 


----------

[歌中文开发者博客原文](http://developers.googleblog.cn/2017/08/android-things-developer-preview-5.html)