# README

§1 – Introduction to Linear Programming Synopsis •What is mathematical optimisation? •What is linear programming? •What do we mean by linear _constraints_ and a linear _objective function_?

§2 – The Geometry of Linear Programming Synopsis •What is a _feasible region_? 可行域 •How do we obtain the optimal solution via the _graphical method_? 如何通过图形方法获得最佳解决方案 •Are there _pathological cases_?

§3 – The Geometry of LP in Higher Dimensions Synopsis •What are _convex sets_? •What is a _hyperplane_? •What is a _halfspace_? •What is linear independence? 什么是线性独立性？ •What is a polytope? 什么是多表位？ •How do we get from standard form to canonical form?如何从标准形式转换为规范形式？ •What are _slack variables_?

§4 – Basic Feasible Solutions 基本可行域 Synopsis •What is a _basic feasible solution_ \(bfs\); \[Standard Form/Canonical Form\] •_Extreme points_ correspond to basic feasible solutions, and viceversa.

§5 – _Fundamental Theorem of Linear Programming_ Synopsis •Fundamental theorem of Linear Programming

§6 – Preview of the _Simplex Method_ 单纯形法 Synopsis •Methods for solving LPs •Idea of the Simplex Method •An example •The Simplex Method

§7 – The Simplex Method Input:A max Linear Program instandard form Output:An optimal solution 1:Construct canonical form and obtain abasic feasible solution 2:whileThere are negativereduced costsdo 3:Select entering variable with most negative reduced cost. 4:Select leaving variable using theratio test. 5:Pivotthe tableau. 6:end while Here the reduced costs are the coefficients of the variables when we write the objective function as an equation such that all termsare on the same side and the coefficient of z is equal to 1.

To come... •Initialisation 初始化 •Streamlining the process 简化流程 •Optimality test 优化测试 •Iteration 迭代 •LP with no feasible solutionLP，没有可行的解决方案 •LP with no optimal solutionLP 没有最佳解决方案 •LP with multiple optimal solutions 具有多种最佳解决方案的LP

§8 – Solution Possibilities We saw before that linear programming problems can have •multiple optimal solutions, •an unbounded objective function, or •an empty feasible set. We want to know how to recognise these situations when using the Simplex Algorithm.

§9 – Non-Standard Formulations Recall that the Simplex Algorithm relies very much on theCanonical Form, which, in turn, requires the correct Standard Form, that is, •the optimisation criterion is opt= max, •all RHS coefficients are nonnegative, •all functional constraints are “≤” type inequalities \(whichensuresmslack variables in the initial tableau and so theinitial bfs\), and •all variables are nonnegative. Not all programs can be written in Standard Form. So extra stepsare needed to convert such programs to the Canonical Form. here are 5 scenarios we must deal with: •we have a minimisation problem; •a variable is unrestricted in sign \(urs\); •some part ofb= \(b1,...,bm\)is negative; •we have a “≥” constraint; •we have a “=” constraint.

§10 – Duality Theory 对偶理论 Duality is a very elegant and important concept within the field ofoperations research, just as in many other branches ofmathematics. In operations research, the theory of duality was first developed inrelation to linear programming, but it has many applications, andperhaps even a more natural and intuitive interpretation, in severalrelated areas such as nonlinear programming, network optimisationand game theory. 就像在数学的许多其他分支中一样，对偶性是运筹学领域中一个非常优雅而重要的概念。 在运筹学中，对偶理论最初是与线性规划有关的，但在非线性规划，网络优化和博弈论等几个相关领域中，它具有许多应用，甚至可能更自然，直观。 Every linear program has associated with it a related linearprogram called its _dual_. When we are talking about the dual wecall the original problem the _primal_.

§11 – Sensitivity Analysis 敏感性分析 So far we have assumed that the various parameters that describea linear programming problem are all given. However, in real life, this is rarely the case. For example, we mighthave only an estimate of the profit that we can make on each ofour products. In such situations we want to know how the solution to a linearprogramming problem will vary if the parameters change. Sensitivity Analysis is the subject which deals with these issues.This section is intended to be a very brief introduction to Sensitivity Analysis. Ingredients of LP Models: •A linear objective function •A system of linear constraints ◦RHS values ◦Coefficient matrix \(LHS\) ◦Signs \(=,≤,≥\)

## Notes

☄︎ Linear Programming Problems Decision Variables && Objective question && Constraints **Formulation:** m denote the number of _functional constraints_\(functional constaints表示是事件里的供需条件, 不包括整数/非负\) n denote the number of _decision variables_ bi denote the available level of resource i, i= 1,2,3,...,m xj denote the level of activity j, j= 1,2,3,...,n z denote the value of the _objective function_ cj denote the return/cost per unit of activity j aij denote the amount of resource i consumed /produced by each unit of activity j. **Assumptions** ¶ Activity levesl are continuous \(divisibility\). LP里假设是continue的 ¶ \(dv\) is proportional to the event. ¶ Independence of the effects of event \(additivity\). ¶ The input parameters are known withcertainty.

**Feasible region** Definition: the set of all feasible solutions of a LP problem

**Graphical Method** ¶ The graphical method can be used to identify the hyperplanes specifying the optimal solution. ¶ The optimal solution itself is determined by solving therespective equations. ¶ The optimal solution in this example is an extreme point ofthe feasible region.

**Pathological cases** 特殊情况 ¶ Infinitely many solutions ¶ Infeasibility ¶ LP is unbounded ¶ Feasible region is not closed »»» 考试不包括 在练习的时候讨论

¶ Convex **Convex combination** w=α₁x₁+α₂x₂+...+αkxk; 0≤αi≤1and ∑iαi= 1, $\displaystyle ⋂\_{i=1}ˆn$ ℂi

¶ **Hyperplane** A set of points H⊆Rⁿ satisfying a linear equation of the form a₁x₁+a₂x₂+...+anxn=b, for\(a₁,a₂,...,an\)≠ \(0,0,...,0\), is a hyperplane.

> Hyperplanes are of dimension \(n−1\). \(Why?\)

¶ **half-spaces** The two closed **half-spaces** defined by the hyperplane a₁x₁+a₂x₂+...+anxn=b, are the set defined by a₁x₁+a₂x₂+...+anxn≥b\(positive half space\) and a₁x₁+a₂x₂+...+anxn≤b\(negative half space\).

> Hyperplanes and their half-spaces are convex sets. Proof

¶ A polyhedron is a non-empty bounded polytope. 多面体是非空有界多面体。

Extreme point: 当我们得出x =λy+（1-λ）z，with y，z∈ℂ and 0&lt;λ&lt;1，then y = z = x时, 凸集ℂ的一个点x就是ℂ的extreme point/vertex. 从几何上讲，这意味着没有点y和z in ℂ\(different from x\)on line segment连接y和z

**Linear Independence** A collection of vectors x\(1\),...,x\(s\)inRn is said to be linearly independent if α₁x₁+α₂x₂+...+αkxk = 0; implies that α₁=α₂+...+αk. Geometrically this means that 集合中的任何向量都不能表示为集合中其他向量的线性组合。

**Theorem** ![avator](../../../.gitbook/assets/theorem1.png) proof 根据定义，多面体是有限个半空间的交集。我们已经看到 •半空间是凸集， •任意数量的凸集的交集都是凸集。多面体是凸的这一事实遵循。

![avator](../../../.gitbook/assets/theorem2.png) 如果线性规划问题恰好有一个最佳解，那么这个解必须是可行区域的一个极点。 proof 我们将通过矛盾来证明这个定理。

如果线性规划问题具有多个最优解，则它必须具有无限多个最优解。此外，最优解集是凸的。

**Standard Form** Canonical Form slack variables When a slack variable takes the value zero, the correspondinginequality issatisfied with equality.

## Basic Feasible Solutions\(bfs\)

Extreme points correspond to basic feasible solutions, and _vice versa_.

**Fundamental theorem** of Linear Programming Corollary 5.1 If the feasible region of the linear programming problem is notempty then it must have at least one extreme point. Corollary 5.2 The feasible region possesses at most a finite number of extremepoints \(Can you suggest an upper bound?\) Corollary 5.3 If the linear programming problem possesses an optimal solution,then there is an optimal solution which is an extreme point of thefeasible region.

**Simplex Method**

思想：定点之间的转移，逐步优化函数

1&gt; 初始点 \(直接观察，松弛变量“≤的s.t.”，人工变量“≥d的s.t.”\)

2&gt; 判别是不是最优

