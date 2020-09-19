# MAST20018 Discrete Maths and Operations Research

\[toc\]

> 课程纵览 MAST20018 引入了运筹学方法的基本特征，还引入了离散数学领域，重点关注应用程序。运筹学主题包括数学模型，线性规划，单纯形方法和对偶理论。离散数学主题包括调度，图论，分配和匹配以及公平分配。主题材料的共同主题是在商业环境，行业和日常生活中遇到的现实环境中的数学应用。

## Overview

[LP Solver](https://online-optimizer.appspot.com/?model=ms:iTMWsDyaxslDogEc1on6BK409a0JEI8K) & [Operation Research](https://www.notion.so/Operations-Research-49dd3e13f6944a77bad9aa5e9711d04a) & [Roam Research](https://roamresearch.com/#/app/courses) & [Perusall](https://app.perusall.com/home) MAST20018 introduces the essential features of operations research methods, and also introduces the area of discrete mathematics with a focus on applications. Operations Research topics include mathematical modeling, linear programming, simplex method, and duality theory. Discrete Mathematics topics include scheduling, graph theory, assignments and matchings, and fair devision. The subject material has a common theme of applications of mathematics in realistic settings encountered in the business world, industry and day-to-day life.

### 🏫Learning Outcomes

**LO1:** Comprehend the essential features of problems encountered in operations research investigations, as well as those encountered in applied discrete mathematics. **LO2:** Develop basic skills required to construct formal mathematical models for practical optimization problems, and those required to analyze settings from real-world applications. **LO3:** Appreciate the extent and limitations of a number of operations research and discrete mathematics techniques for solving real-world problems.

### 🔧General Skills

**GS1:** Problem solving skills: the ability to engage with unfamiliar problems and identify relevant solution strategies. **GS2:** Analytical skills: the ability to construct and express logical arguments and to work in abstract or general terms to increase the clarity and efficiency of analysis. **GS3:** Collaborative skills: the ability to work in team. **GS4:** Time management skills: the ability to meet regular deadlines while balancing competing commitments.

## Assignments 🧨

[Assgnment](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/Ass/Assesment.md) 20% & [Final](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/Ass/Final.md) 80%

## Course Notes

Part1: Operations Research

#### Week\_01: [mathematical modeling in linear programming and the graphical method](https://www.notion.so/week-1-mathematical-modeling-in-linear-programming-and-the-graphical-method-9f8e95e617e24cfda04bdfe9ab1853ce)

§1 – Introduction to Linear Programming Synopsis •What is mathematical optimisation? •What is linear programming? •What do we mean by linear constraints and a linear objective function? •什么是数学优化？ •什么是线性编程？ •线性约束和线性目标函数是什么意思？

#### [Week\_02: the algebra of linear programming](https://www.notion.so/week-2-the-algebra-of-linear-programming-efcbba21c1a244f2bdc6a9388e278204)

[Tutorial01](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/Turorial/tutorial01.pdf) §2 – The Geometry of Linear Programming Synopsis •What is a feasible region? •How do we obtain the optimal solution via the graphicalmethod? •Are there pathological cases? 概要 •什么是可行区域？ •如何通过图形方法获得最佳解决方案？ •是否有特例？ §3 – The Geometry of LP in Higher Dimensions Synopsis •What are convex sets? •What is a hyperplane? •What is a halfspace? •What is linear independence? •What is a polytope? •How do we get from standard form to canonical form? •What are slack variables? •什么是凸集？ •什么是超平面？ •什么是半空间？ •什么是线性独立性？ •什么是多表位？ •如何从标准形式转换为规范形式？ •什么是松弛变量？ §4 – Basic Feasible Solutions Synopsis •What is a basic feasible solution \(bfs\); •Extreme points correspond to basic feasible solutions, and viceversa. •什么是基本可行的解决方案（bfs）； Standard Form/Canonical Form •Extreme points对应于基本可行的解决方案，反之亦然。

#### [Week\_03: solving linear programming problems and introduction to the simplex algorithm](https://www.notion.so/week-3-solving-linear-programming-problems-and-introduction-to-the-simplex-algorithm-2e3df5b5703c4628b0ff2e40dcd3a9e1)

[Tutorial02](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/Turorial/w3_tutorial_sheet_2020.pdf) §5 – Fundamental Theorem of Linear Programming Synopsis •Fundamental theorem of Linear Programming §6 – Preview of the Simplex Method 单纯形法 Synopsis •Methods for solving LPs •Idea of the Simplex Method •An example •The Simplex Method

#### [Week\_04: diving in the simplex algorithm](https://www.notion.so/week-4-diving-in-the-simplex-algorithm-0a89e1cd1f104088ab11b3409a4058b3)

[Tutorial03](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/MAST20018/Turorial/20018w4-2.pdf) §7 – The Simplex Method Input:A max Linear Program instandard form Output:An optimal solution 1:Construct canonical form and obtain abasic feasible solution 2:whileThere are negativereduced costsdo 3:Select entering variable with most negative reduced cost. 4:Select leaving variable using theratio test. 5:Pivotthe tableau. 6:end while Here the reduced costs are the coefficients of the variables when we write the objective function as an equation such that all termsare on the same side and the coefficient of z is equal to 1.

To come... •Initialisation •Streamlining the process •Optimality test •Iteration •LP with no feasible solution •LP with no optimal solution •LP with multiple optimal solutions

§8 – Solution PossibilitiesWe saw before that linear programming problems can have •multiple optimal solutions, •an unbounded objective function, or •an empty feasible set. We want to know how to recognise these situations when using the Simplex Algorithm.

§9 – Non-Standard Formulations Recall that the Simplex Algorithm relies very much on theCanonical Form, which, in turn, requires the correct Standard Form, that is, •the optimisation criterion is opt= max, •all RHS coefficients are nonnegative, •all functional constraints are “≤” type inequalities \(whichensuresmslack variables in the initial tableau and so theinitial bfs\), and •all variables are nonnegative. Not all programs can be written in Standard Form. So extra stepsare needed to convert such programs to the Canonical Form. ![avator](../../.gitbook/assets/standardform.png) here are 5 scenarios we must deal with: •we have a minimisation problem; •a variable is unrestricted in sign \(urs\); •some part ofb= \(b1,...,bm\)is negative; •we have a “≥” constraint; •we have a “=” constraint.

§10 – Duality Theory 对偶理论 Duality is a very elegant and important concept within the field ofoperations research, just as in many other branches ofmathematics. In operations research, the theory of duality was first developed inrelation to linear programming, but it has many applications, andperhaps even a more natural and intuitive interpretation, in severalrelated areas such as nonlinear programming, network optimisationand game theory. 就像在数学的许多其他分支中一样，对偶性是运筹学领域中一个非常优雅而重要的概念。 在运筹学中，对偶理论最初是与线性规划有关的，但在非线性规划，网络优化和博弈论等几个相关领域中，它具有许多应用，甚至可能更自然，直观。 Every linear program has associated with it a related linearprogram called its _dual_. When we are talking about the dual wecall the original problem the _primal_.

§11 – Sensitivity Analysis 敏感性分析 So far we have assumed that the various parameters that describea linear programming problem are all given. However, in real life, this is rarely the case. For example, we mighthave only an estimate of the profit that we can make on each ofour products. In such situations we want to know how the solution to a linearprogramming problem will vary if the parameters change. Sensitivity Analysis is the subject which deals with these issues.This section is intended to be a very brief introduction to Sensitivity Analysis. Ingredients of LP Models: •A linear objective function •A system of linear constraints ◦RHS values ◦Coefficient matrix \(LHS\) ◦Signs \(=,≤,≥\)

#### Week\_05: duality and sensitivity analisis

#### [Week\_06: wrap up on linear programming](https://www.notion.so/week-6-wrap-up-on-linear-programming-3589ecccfced42bea0744da43de1aab3)

Part2: Discrete Mathematics

#### [Week\_07: schedulling](https://www.notion.so/week-7-schedulling-7673ad7f9efe4cbd8abb3ff152c12c88)

#### [Week\_08: network optimisation](https://www.notion.so/week-8-network-optimisation-ce4af7a03cdf46f2926bd2b3d099ba2e)

#### [Week\_09: network optimisation](https://www.notion.so/week-9-network-optimisation-c68ca4233ed2439c856a455b652490f5)

#### [Week\_10: social choice](https://www.notion.so/week-10-social-choice-691ed5f2ccbc4fcbb5d50e768bc2b509)

#### [Week\_11: social choice](https://www.notion.so/week-11-social-choice-88915484e07941e2a49403d757b089a4)

#### [Week\_12: review and preparation for exam](https://www.notion.so/week-12-review-and-preparation-for-exam-1846b9477f4f4fd6a2bcfdb46a6c405a)

## Relational Knowledge / Resourses

Youtube Lecture of Linear Programming

[Linear Programming, Lecture 1. Introduction, simple models, graphic solution](https://www.youtube.com/watch?v=FdKgeeb4q3w&list=PLbxFfU5GKZz1Tm_9RR5M_uvdOXpJJ8LC3)

## Reference && More Details

This page copyied from -- [MAST20018 Discrete Maths and Operations Research](https://www.notion.so/MAST20018-Discrete-Maths-and-Operations-Research-57b79741c0454ec4bbd574622f364da1) designed Haoyu\_Huangsun  
 Courses Imormation by Univerity of Melbourne

