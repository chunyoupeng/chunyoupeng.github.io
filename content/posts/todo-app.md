---
title: My Personal TODO App
author: Chunyou Peng
date: 2024-03-02
description: TODO App 构建思路
tags: ["tech"]
type: "post"
---

# TODO-APP

## 需求

### 软件思路

这个app用来管理用户的todo事项。

用户可以添加，修改，删除事项。每个事项有一个优先级，1－5星。优先级最高的排在最前面。用户点击事项前面的已完成按扭之后，就会被移到已完成的一个箱子里面。用户可以选择点击这个箱子查看。

### 前端

前端使用vite 创建react项目.使用ts.css使用tailwincss

按扭有添加,删除,已完成,设定优先级(1-5).完成箱(用来查看已完成的事项)
并且显示添加的日期

### 后端

数据库使用postgresql

内容有 
完成情况(已完成/未完成) | 事件 | 优先级 | 添加的日期

