---
title: My Master Theorem Understanding
author: Chris Penn
date: 2024-04-06
description: my own understanding of mater theorem
tags: ["math"]
type: "post"
---
# Book Screenshot

![pic](/img/master-theorem.png ) 

## My Quick Understanding

就是比较f(n)和$n^{\log{b^a}}$

1. f(n)的阶数要小一点,T(n)=O($n^{\log{b^a}}$)
2. 相同,则是乘以一个log
3. f(n)的阶数要大一点,要判断一个af(n/b) <= cf(n),c<1.如果满足,T(n)=O(f(n))

> 其实就是以大的为主
