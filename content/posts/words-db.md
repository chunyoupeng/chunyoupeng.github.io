---
title: Personal Wrods DB App
author: Chunyou Peng
date: 2024-03-01
description: word app for advanced English learners
tags: ["tech"]
type: "post"
---

# Personal Wrods DB App

## 需求

### 软件思路

这个软件的目的是记录和跟踪用户的词汇情况. 

用户在日常的生活中,可能会遇到一些生词,这个时候就可以把这个单词录入到系统里面.系统首先在数据库里查询这个单词.如果有,则返回查询这个单词的次数和意思.如果没有,则使用一个函数
GetMeaning(word){return word + "meaning is";}, 目前就一个定死的函数.返回他的意思,查询次数设为1.

系统的第二个功能是:用户在读一篇文本的时候,想知道哪些单词不认识.他可以把这篇文章复制到另一个查询框.系统通过查找每一个单词, 如果不在数库里面,系统一行一行输出这些单词的原单词,查询次数,单词意思.


### 前端

使用reactjs.有两个选项, 一个是录单词的.另一个就是录文本的.

下面都有对应的按纽,点击就调用具体的功能.

### 后端

数据库使用postgresql.

内容有
单词 | 查询次数 | 单词意思

