title: 好好玩git之git-config
categories:
  - git
  - git-config
tags:
  - 好好玩git
toc: true
author: 王晓勃
comments: true
date: 2016-11-03 14:15:00
description:
original:
permalink:
---
![](/images/git/0.png)
git是什么？关于git的身世和作用本篇不做赘述，网上相关资料很多，有兴趣的小伙本可以google一下。简单的说git是一个 **分布式** 版本控制软件，和大家熟知的svn一样都是版本控制软件，但是git无论功能和设计理念都先进了很多，特别是这个 **分布式** ！
<!-- more -->

# 我是如何爱上git的？

2014年开始工作，在一家对日外包公司使用svn进行团队代码控制。就记住了Windows上那个🐢，简单了学习了一下如何操作。但是一年多的使用感觉就是那个样，玩不出什么花样！作为一个有想法爱折腾的程序猿当然对svn无感了，后来当我听同事提到版本控制还有一个 **git**，回家立马了解了一下，原来这东西是Linux之父 **Linus Torvalds** 开发出来的，也知道了git和BitKeeper的故事，更加崇拜我神：Linus了！大神就是不给我用这个软件，那我就重新写一个自己的！真是羡慕死我等屌丝，偶像的力量是强大的！虽然我还不知道git到底够不够优秀，但是我已经爱上了它。

# git 配置

说回正题，本片内容主要是演示和记录关于git的配置，以点带面，抛砖引玉。

# 帮助资料

* [github](https://github.com) 最大的代码托管站点，在这里可以找到非常多非常优秀的源代码
* [Pro Git](https://git-scm.com/book/zh/v1) 全面学习git的一本好书
* [try git](http://try.github.io/) 在线学习git相关指令的网站
* [man git](https://www.kernel.org/pub/software/scm/git/docs/) git命令帮助手册（英文）
