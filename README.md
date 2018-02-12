# 订阅阅读器测试
---

## 项目背景

测试是开发流程当中的重要一环，许多组织都实行一套标准的开发程序，称为“测试驱动开发”。即开发人员首先编写测试，然后才开始应用程序开发。所有测试的初始状态都是未通过， 然后开始编写应用程序代码，以通过测试。

无论你工作所在的组织是否实行测试驱动开发,  还是利用测试来确保未来功能开发 不对现有功能造成伤害，测试都是一项重要的必备技能！

## 项目概述

此项目是一个基于 Web 的 RSS 反馈阅读应用程序。显然，测试是很重要的一部分，已在其中包含了 Jasmine，并已编写了**RSS Feeds**，**The menu**，**Initial Entries**，**New Feed Selection** 测试套件，分别负责不同部分的测试。

## 项目分析

* RSS Feeds 测试套件：都是关于 Rss 源的定义的，也就是项目中的 allFeeds 变量

    * 保证 allFeeds 变量被定义了而且不是空的

    * 保证 allFeeds 变量里面所有源的名字字段和链接字段均不为空
    
* The menu 测试套件：关于页面中侧面菜单栏的测试

    * 保证侧面菜单栏默认隐藏，当点击汉堡图标时菜单栏可见，再次点击时，菜单栏隐藏
    
* Initial Entries 测试套件：关于页面中 feed 容器能否正常加载 entry 元素的测试

    * 保证页面中可以正常显示各源的链接
    
* New Feed Selection 测试套件：关于切换菜单栏中源时内容是否改变的测试

    * 保证当切换源时页面内容发生改变

## 测试结果

如下所示，当所有测试均通过时，会显示 0 failures

![测试结果](https://raw.githubusercontent.com/ShiHaiou/Udacity-FeedReaderTesting/master/images/test_result.PNG)

当然可以实验一下这个测试，比如把 app.js 里面的 allFeeds 变量变成一个空的数组然后刷新页面，结果如下所示：

![测试addFeeds](https://raw.githubusercontent.com/ShiHaiou/Udacity-FeedReaderTesting/master/images/test_addFeeds.PNG)

## 参考文档

* [使用jasmine来对js进行单元测试](https://www.cnblogs.com/kbqncf/p/3795155.html)

