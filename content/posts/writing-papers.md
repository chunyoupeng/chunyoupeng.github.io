---
title: How to Write a Paper?
author: Chunyou Peng
date: 2024-03-20
description: notes of the standford cs 197 course
tags: ["papers"]
type: "post"
---

# How to Get Started?

First, find the nearest paper, then its neighbors. Give them topics to write your liturature review.
Find what they have done, and what they didn't. 

# How to read a paper

## Outlining a Paper

Your outline should recompress the paper back into an outline format that explains the paper's argument. We suggest the following structure of one paragraph per bullet, with an example outline following the description:

**Title**: What paper did you read?
**Problem**: What problem is it solving? Why does this problem matter?
**Assumption in prior work**: What was the assumption that prior research made when solving this problem? Why was that assumption inadequate?
**Insight**: What is the novel idea that this paper introduces, breaking from that prior assumption?
**Technical overview**: How did the paper implement that insight? I.e., What did they build, or what did they prove, and how?
**Proof**: How did the paper evaluate or prove that its insight is correct, and is better than holding on to the old assumption?
**Impact**: What are the implications of this paper? How will it change how we think about the problem?

## Example

**Title**: Flash Organizations: Crowdsourcing Complex Work by Structuring Crowds As Organizations
**Problem**: Crowdsourcing has been used successfully for many goals that can be decomposed into small, modular microtasks, but it has struggled to achieve more complex goals such as design and engineering. For example, tasks such as image labeling work because it's modularizable, but design is interdependent and requires adapting as you go, so crowdsourcing has succeeded at image labeling but failed at design. If crowdsourcing is limited to modular tasks, then it will never be able to achieve goals of meaningful complexity, which will limit its impact on the world.
**Assumption in prior work**: Prior work all takes an algorithmic model of crowdsourcing: the programmer specifies who does what, and when, in a kind of big algorithmic recipe to follow. This assumption shows up in goals ranging from Wikipedia ("edit this page"), to interactive crowd-powered interfaces ("find errors" --> "fix errors" --> "verify fixes"), to open source software ("create a module with this fixed API").
**Insight**: This paper proposed that instead of coordinating crowds as we do algorithms, that we should be coordinating crowds as we do with organizations. They propose a series of computationally-enhanced versions of the structures that organizations use — roles, tasks, hierarchy, and so on — and introduce the idea of a flash organization, which is a rapidly assembled collective of online collaborators who use these computational organizational structures to coordinate.
**Technical overview**: The authors created a system called Foundry that implements these ideas. Foundry is a web interface that connects to the Upwork online labor marketplace to draw on-demand expertise. It uses a combination of first-come-first-served hiring queues and Slack integration to bring workers onboard and keep them updated. It introduces an adaptation model drawn from the metaphor of code branching and merging to enable the organization to adapt.
**Proof**: Three non-crowdsourcing experts used the system to convene and lead flash organizations to achieve proof-of-concept complex goals. These experts created (1) a tablet system for EMTs to report medical trauma cases enroute to the hospital, (2) a card game for storytelling, which was playtested and iterated upon, and (3) an enterprise-grade event planning system that had to meet branding and security standards.
**Impact**: Flash organizations offer a broad new view of crowdsourcing — one that's not rooted in Tayloristic algorithms, but instead in an organizational metaphor. This approach can achieve far more complex outcomes, enabling crowdsourcing to apply to a broad new class of problems. It has implications for the future of work (how do we protect labor rights?), for organizations (what will organizations look like in the future if flash organizations are widely deployed?), and for collaboration (will we all work remotely?).

# Whats introduction

The introduction part  of  a paper  is to convey my research to others. I should be able to explain twe things, the one is to explain what I am doing, the other is to explain the importance of my work.

### The Architechture of an intro

- Problem

前人遇到的一些挑战,可以写一些综述

- Solution

Your big idea + instantiate and concrete your idea

总结成一句,找文献发现问题并且设置一个点.然后讨论自己的方法或者模型能够解决这个问题.

**两种结构**:

New promblem / old solution

Old problem / new solution

- Motivate the problem via rhetoric, drawing on prior work making supporting claims
- Set up the bit: prior work is not equipped for this problem
- Flip the bit — how your approach draws on known ideas Instantiate that solutionImplications

Old problem / new solution:

- Motivate the problem via prior work, which has already established the problem
- Set up the bit of how all prior work tried to solve it
- Flip the bit — your new solution. Instantiate that new solution. Implications
> Address a new problem with a new solution is hard to convince the world. 


# Vectoring and Velocity

**Vectoring**: identifying the biggest dimension of risk in your project right now
>选择优先级最高的问题去解决.从一个维度去解决.如果解决不了,就进行跌代,解决下一个问题.

**Velocity**: rapid reduction of risk in the chosen dimension


## Core-periphery mindset

Vectoring helps us find the good question, the next step is to answer the question. 把自己所有的能量集中于解决那个问题,谈化其它的部分,以解决这个问题为主要的动力.
> The week’s goal is instead an answer to a question. To answer a question, you don’t need to address all the issues in the periphery. Just focus on what’s in the core.

### Test

一定要选择最核心的部份进行测试。选择最小块，然后把其它关联性小的部份忽略掉。
