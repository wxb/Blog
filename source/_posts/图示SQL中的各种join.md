title: 图示SQL中的各种join
categories:
  - null
tags:
  - null
toc: true
author: 王晓勃
comments: true
date: 2016-12-15 10:27:11
description:
original:
permalink:
---

数据库中的`join`成为**连接**，连接的主要作用是根据两个或多个表中的列之间的关系，获取存在于不同表中的数据。连接分为三类：**内连接**、**外连接**、**全连接**

<!-- more -->

# 上图
![](/images/mysql/01.jpg)
***图片来自网络***

# 数据准备

```sql
CREATE DATABASE join_test CHARSET UTF8;

CREATE TABLE `Persons` (
  `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
  `LastName` char(16) NOT NULL DEFAULT '',
  `FirstName` char(16) NOT NULL DEFAULT '',
  `Address` varchar(128) NOT NULL DEFAULT '',
  `City` varchar(128) NOT NULL DEFAULT '',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

CREATE TABLE `Orders` (
  `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
  `OrderNo` int(11) NOT NULL DEFAULT '0',
  `Pid` int(11) NOT NULL DEFAULT '0',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

```

# 内连接(图-3)


# 外连接(图-1、2)

# 全连接(图-4)
