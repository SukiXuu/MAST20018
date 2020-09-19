# week03

Recap：

## Standard Form:

要求条件： 1. 2. 3. 4.

一般形式：

转换练习：

## Canonical Form: 所有LP的都可以达成\(用Xj≥0来把不等式转为等式子\)

一般形式：

Slack Variable： 松弛变量, 补足了左边比右边少的部分 if Xslack = 0 就说明不是不等式，本身就是等式

转换练习（2015 （2）b）：

如何从 Canonical form 中找 Feasible Solution？

注意：Feasible 不一定代表optimal 1. 2.

例子：

Basic Solution：

Basic Feasible Solution： 对应关系

Note： 对应关系：

## Simplex Algorithms：----- 解LP的方法

原理： BFS ⬄ Optimal ⇰ 逻辑：

Initialisation：

Iteration：

1. Entering Variable：
2. Leaving Variable
3. Pivot

Termination：

例题：

验算： 1. 2.

## Assignment 思路解析

Q1. 行动调查 决策理论 基本可行的解决方案 松弛变量 凸集 分配问题 建议： Operations research Decision theory Basic feasible solution Slack variable Convex set The assignment problem

示范： 是什么 用来干什么 有什么构成 slack V：在优化问题中 ，添加到inequality constraints 上的变量， 能把不等式constraint 转化为等式constraint，代表了standard form中不等式两边的差值 和

Q2 用LP解决球员首发问题 Xij 球员i打不打位置j Cij 合适程度 N 球员 M 位置

