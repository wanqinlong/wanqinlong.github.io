---
title: 《Android | 译文：现代Android开发入门资源》
date: 2017-9-14 17:20:49  #文章生成时间
categories: #法律法规 #文章分类目录 可以省略 
- Android
- # 分类2
tags: #文章标签 可以省略 #设置为则当前页没有打赏按钮reward: false
- # 标签1    #  正文截取<!--more-->
- # 标签2
---
![](https://i.imgur.com/7pfitW2.png)

<!--more-->

[原文](https://riggaroo.co.za/resources-getting-started-android-development/) 
**
[现代ANDROID开发入门资源](https://riggaroo.co.za/resources-getting-started-android-development/)

由Franks.Rebecca |2017年8月14日**

在将我们在DVT上运行的移动开发人员研究生课程的资源整合后，我意识到我引用的内容可能是开始使用Modern Android开发的好手段。

值得注意的是，我们有一个非常实际的方法来训练DVT的毕业生。我们举办研讨会和实际项目，以确保我们的毕业生对Android开发有了坚实的了解。

随着大量的在线内容的可用性，当我开始Android开发时，我并不知道在哪里看，或者在开发应用程序时应该注意什么。在这篇博客文章中有一个简明的列表，对我而言是非常宝贵的。我希望你也能发现它的价值。

这是一个链接，代码实验室和参考资料的列表，对于任何希望在Android开发领域开始使用的开发人员将是有用的。

# 一般编程实践 #
以下一般编程实践是您成功开发事业的关键。这些做法包括：

 - 源代码控制（Git）  - 源代码管理是一种管理代码版本的工具，它非常适合协同编写软件。
 - Git工作流程  - 使用源代码管理时，有许多不同的方式来管理软件。流行的方法包括：Gitflow工作流程，集中式工作流程，分岔工作流程
 - 持续集成  - 持续集成确保您的代码建立在不是您自己的机器的服务器上。看看使用像Jenkins，Buddybuild，Circle CI，Travis等的构建服务器
 - 拉请求  - 拉请求是一个很好的方式来获得关于您开发的代码的非常详细的反馈。
 - 敏捷/ Scrum方法  - 大多数现代软件开发团队遵循Scrum方法进行工作。
 - 代码质量工具 - 公司使用许多工具来衡量其代码的质量和代码库的运行状况。诸如测试覆盖的行数或代码库具有多少技术债务的指标变得可见。一些常用的工具：Sonar，FindBugs，Checkstyle和Android Lint。

# Android基础介绍 #
有一些网站提供开始使用Android开发的基础知识。我的建议是遵循正式文档来了解基础知识，然后查看其他资源（例如博客等），以获取更多信息，以了解更多应用设计的技术方面（参见本文后面的部分）。

## 一些入门资源： ##

 - Android应用基础知识
 - Android中的一些主要组件：活动，片段，服务，广播接收器。
 - Android应用程序清单
 - 代码实验室 - 构建您的第一个Android应用程序

# 掌握Android中的布局 #
Android中有很多不同的布局类型，从FrameLayout到RelativeLayout到ConstraintLayout。确保你喜欢这些常用的布局类型：FrameLayout，RelativeLayout，LinearLayout，ConstraintLayout，CoordinatorLayout。

## 资源： ##
 - 支持不同的屏幕尺寸
 - 代码实验室 - 约束力
 - 代码实验室 - CoordinatorLayout

# 构建系统 - 使用Gradle #
使用Gradle可能是在开发Android应用程序时被忽略的东西。确保您了解基础知识，更好 - 了解如何编写自己的毕业生任务！

## 资源： ##
 - Gradle文档
 - 配置您的Build

# Android中的网路 #
虽然大多数的Android文档都没有引用Retrofit或者OkHttp，但是在Android中的网络连接中，这些都是最常用的库。熟悉Android Studio中可用的不同的分析工具也很好。

## 资源： ##

 - 了解RESTful服务
 - 改装 - 适用于Android和Java的类型安全的HTTP客户端
 - OkHttp  - 适用于Android和Java应用程序的HTTP＆HTTP / 2客户端
 - Android中的网络Profiler  - Android Studio中的一个工具，可让您配置网络呼叫。
 - Charles Proxy  - 用于在测试时拦截网络呼叫。

# 构建您的Android应用程序 #
不幸的是，编写代码并让应用程序编译不知道如何编写可维护的Android应用程序。大规模的Android应用程序需要遵循良好的架构设计，以使它们可维护和可测试。编写Android应用程序时可以遵循许多不同的模式。通常使用MVP，MVVM和Clean Architecture等模式。确保您了解模式之间的差异，因为您将在野外遇到许多不同的模式。

## 资源： ##

 - Android架构组件指南
 - 我在Android体系结构组件3部分组成的系列（部分1，2，3）
 - Android架构组件视频介绍
 - Google示例应用程序Github Repository
 - 代码实验室 - 持久性
 - 代码实验室 - 生命周期意识组件

# 测试您的Android应用程序 #
一旦创造出Android应用程序，您将需要考虑如何测试它们。单元测试和UI测试是您需要确保理解的非常重要的概念。您可以使用大量不同的工具来编写UI测试。大多数Android开发人员使用Espresso和JUnit编写测试，但还有许多其他工具，如Robotium，Calabash，Appium等。我建议使用Espresso和JUnit。

## 资源： ##

 - Android测试支持库
 - 浓咖啡
 - JUnit的
 - 的Mockito
 - 代码实验室 - Android测试
 - 代码实验室 - Android性能测试

# 发布您的Android应用程式 #
太好了，你已经做到这一点了！现在有几个概念，您需要覆盖才能发布您的应用程序：

 - 准备您的应用程序发布
 - 应用程序签名
 - 版本化您的应用程序
 - ProGuard的

# 安全 #
为了保护您的应用程序，确保没有人可以访问未经授权的内容，应该做很多事情。确保使用ProGuard（前面提到）。了解中间人的男人是谁。了解不同的加密方式和方法，您可以将信息安全地存储在Android应用程序中，包括保护您的API令牌，证书固定等。

## 资源： ##

 - Android上的安全提示
 - 证书固定
 - SafetyNet API
 - Android Keystore系统

# 高级Android主题 #
一旦涵盖了编写Android应用程序的所有基础知识，您可能需要覆盖几个高级主题，以便为某些代码库做出贡献：

 - Kotlin  - Kotlin是Android的新编程语言，开发人员正在Kotlin编写代码。值得一读关于科特林，并通过科特琳·科恩（Kotlin Koans）。还有一个Kotlin代码实验室可用。
 - RxJava  -  RxJava是用于异步，基于事件的编程的库。它允许您组合操作在一起以执行复杂的任务（例如将多个网络调用组合在一起），并且对于管理执行代码的线程可能非常有用。来自Jake Wharton的精彩视频介绍了如何使用RxJava以及使用它的好处。
 - Dagger（依赖注入） - 依赖注入是一种在应用程序中管理对象及其依赖关系的方法。DI的概念不是Android，而是在许多其他框架中可用。DI可以使您的代码更高效地记忆，并提高可测试性。Dagger 2是最受欢迎的Android DI框架。
 - 材料设计  - 大多数Android应用遵循Google的材料设计指南。指南是以用户习惯的标准方式设计您的应用程序的一种方式。
 - Android中的支持库  -  Android中的支持库非常重要，可确保您的应用程序在多个版本的Android中保持一致。有几个不同的图书馆有不同的目的。链接的文章描述了图书馆背后的原因。
 - 内存泄漏 -  在Android中，创建内存泄漏非常容易。这可能导致应用程序中的错误行为（随机崩溃）。阅读这里的内存泄漏。许多开发人员在他们的应用程序中使用LeakCanary来确保没有任何内存泄漏。
