title: 高性能MySQL-EXPLAIN
categories:
  - 数据库
tags:
  - MySQL
  - 性能优化
toc: true
author: 王晓勃
comments: true
date: 2016-07-03 17:46:05
description:
original:
permalink:
---
EXPLAIN 句法能够帮助我们了解 MySQL是如何处理 `SELECT`查询操作的；了解一条查询语句执行的过程，提供有关表如何联结和以什么次序联结的信息。

<!-- more -->

# 句法

```mysql
EXPLAIN tbl_name
```
这种用法和`DESCRIBE tbl_name`,`SHOW COLUMNS FROM tbl_name`的作用是一样的

```mysql
EXPLAIN SELECT select_options
```
这种用法，MySQL解释它将如何处理SELECT，提供有关表如何联结和以什么次序联结的信息。

# 作用

借助于EXPLAIN，可以知道什么时候必须为表加入索引以得到一个使用索引找到记录的更快的SELECT。也能知道优化器是否以一个最佳次序联结表。为了强制优化器对一个SELECT语句使用一个特定联结次序

例如：


# 输出信息

* table

* type

* possible_keys

* key

* key_len

* ref

* rows

* Extra
