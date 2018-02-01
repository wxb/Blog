---
title: python的类属性和实例属性
categories:
  - null
tags:
  - null
toc: true
author: 王晓勃
comments: true
date: 2018-02-01 11:29:58
description:
original:
permalink:
---

<!-- more -->

```python
class Student(object):
    age = 18
    yy = []
    params = dict(where='xian')

    def __init__(self, name):
        self.name = name
        #self.params = dict(where='xian')
        print id(self.name)

    def preparams(self, params):
        #self.params = params
        print id(params), id(self.params)
    

stu_a = Student('wangxiaobo')
stu_b = Student('Michael')

stu_a.preparams({})
stu_b.preparams(dict())

```