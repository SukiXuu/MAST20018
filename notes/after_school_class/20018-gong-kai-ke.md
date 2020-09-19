# 20018 公开课

\[TOC\]

## Linear programming optimisation  -&gt;   最优化问题

* 分配问题
* 运输问题
* 最大最小利润
* 等... 

### Optimisation 的构成

1. Decision Variable
2. Objective Function 计算最大/最小值的公式
3. Constraints
   * Functional constraints
   * Demand / resource \(需求&gt;= && resource&lt;=\)
   * non-funcitonal constraint / non-negative 实际意义 & 为了算法

### Notation

* m
* n
* b
* xj
* z
* Cj : xj 的系数「cost」
* Aij: matrice -- coeficient matrices 的 entry

## 四个Assumption --- discuss limitation

* 可分性 divisibility ---- xj 趣取值的连续性
* proportional 成比例性 ----- 不考虑discount
* additionality 可相加 ----- 不存在多个就减少 1个巧克力=100卡路里, 那么 5个就是500卡路里
* certainty 准确性 ------ 系数准确

e.g. Activity levels are not continue

​ The contribution of the object function from DV might not be proportional --- e.g. package deal

​ Activities are not independent --- e.g. digestion system 消化

​ There will be natural variation of wateriest which cause uncertainty

## Geometry

Feasibility:

​ feasible solution: 满足所有constraints

solution:

1. 画图 所有满足的条件
2. 画出z的点
3. 写答

[Hint](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/notes/after_school_class/计算算式要对齐/README.md): 画图注意事项和正常的数学画图是一样的; z的方向; 写答

## Convex combination

​ W = sum of ai \* xi

​ ai belong to \[0,1\] && Sum of a = 1

C Rˆn is

#### ^ω^   //

Useful theorem:

The intersection of ant finite number of convex sets is a convex set.

