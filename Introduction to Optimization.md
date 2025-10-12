> Fix a matrix $\mathbf{A}$. The notation $\mathbf{A}\in M_{m\times n}(\mathbb{R})$ means that $\mathbf{A}$ has $m$ rows and $n$ columns with real-valued entries. The notation $\mathbf{A}(i,j)$ stands for the entry of $\mathbf{A}$ in the $i$-th row and the $j$-th column. The notation $\mathbf{A}(i,-)$ stands for the $i$-th row of $\mathbf{A}$. Likewise, the notation $\mathbf{A}(-,j)$ stands for the $j$-th column of $\mathbf{A}$.
> 
> Fix a column vector $\mathbf{x}$. The notation $\mathbf{x}(i)$ stands for the $i$-th entry of $\mathbf{x}$.

We fix a *linear program* in *standard form* about minimizing a quantity $\mathbf{c}^T\mathbf{x}$, called the *objective function*, with $\mathbf{x}$ satisfying the *equality constraint* $$\mathbf{Ax}=\mathbf{b},$$the *non-negativity constraint* $$\mathbf{x}\geq\mathbf{0},$$
and the *full-rank assumption*: $\mathbf{A}$ as more columns than rows and all rows of $\mathbf{A}$ are linearly independent. The column vectors $\mathbf{x}$ and $\mathbf{c}$ are of size $n$. The matrix $\mathbf{A}$ is of size $m\times n$ (so $n>m$ by the full rank assumption), and so the column vector $\mathbf{b}$ is of size $m$.

## Basic and Feasible Solutions
---
Since rows of $\mathbf{A}$ are linearly independent, we can construct a nonsingular matrix $\mathbf{B}\in M_{m\times m}(\mathbb{R})$ with columns from columns of $\mathbf{A}$. The unique solution to the system $$\mathbf{B}\mathbf{x}=\mathbf{b}$$is then called a *basic solution* for the program with respect to $\mathbf{B}$. If $\mathbf{A}(-,i)$ is a column in $\mathbf{B}$, then the entry $\mathbf{x}(i)$ is called a *basic variable*. If there is a basic variable with value 0, we say that the basic solution is a *degenerate basic solution*.

A solution to both the equality and non-negativity constraint is called a *feasible solution*. A feasible solution that is also basic is called a *basic feasible solution*. A basic feasible solution that is also degenerate is called a *degenerate basic feasible solution*.

## The Fundamental Theorem of Linear Programming
---
A feasible solution that minimizes the objective function is called an *optimal feasible solution*. An optimal feasible solution that is also basic is called a *optimal basic feasible solution*.

The Fundamental Theorem of Linear Programming states that
- if the program has a feasible solution, then the program also has a basic feasible solution, and
- if the program has an optimal solution, then the program also has an optimal basic feasible solution.

## Convex Sets
---
A set of vectors $C$ in $\mathbb{E}^k$ is called *convex* if for all $\mathbf{x}_{1},\mathbf{x}_{2}\in C$ and $\alpha\in (0,1)$ we have $\alpha \mathbf{x}_{1}+(1-\alpha)\mathbf{x}_{2}\in C$. If $C$ and $D$ are convex sets in $\mathbb{E}^k$, then
- for all $\beta\in \mathbb{R}$ the set $$\beta C=\{\beta \mathbf{x}:\mathbf{x}\in C\}$$is also convex and
- the set $$C+D=\{\mathbf{x}+\mathbf{y}:\mathbf{x}\in C\wedge \mathbf{y}\in D\}$$is also convex.

The intersection of any collection of convex sets is also convex.

The smallest convex set containing a set $S$ of vectors in $\mathbb{E}^k$ is called the *convex hull* of $S$, denoted by $\text{co}(S)$. It is the intersection of all convex sets containing $S$.

A set of vectors $C$ in $\mathbb{E}^k$ is called a *cone* if for all $\mathbf{x}\in C$ and $\alpha>0$ we have $\alpha \mathbf{x}\in C$.

A set of vectors $V$ in $\mathbb{E}^k$ is called a *linear variety* if for all $\mathbf{x}_{1},\mathbf{x}_{2}\in V$ and $\alpha\in \mathbb{R}$ we have $\alpha \mathbf{x}_{1}+(1-\alpha)\mathbf{x}_{2}\in V$. A *hyperplane* in $\mathbb{E}^k$ is a linear variety in $\mathbb{E}^k$ with dimension $k-1$. For all column vectors $\mathbf{a}$ of size $k$ and real numbers $c$, the set $$\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}=c\}$$is a hyperplane in $\mathbb{E}^k$. In fact, all hyperplanes in $\mathbb{E}^k$ arises this way.

Given a hyperplane $H=\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}=c\}$ in $\mathbb{E}^k$, we define the *positive closed half space* and the *negative closed half space* associated to $H$ as $$H_{c+}=\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}\geq c\}$$and $$H_{c-}=\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}\leq c\}$$respectively and the *positive open half space* and *negative open half space* associated to $H$ as $$H_{o+}=\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}>c\}$$and $$H_{o-}=\{\mathbf{x}\in \mathbb{E}^k:\mathbf{a}^T\mathbf{x}<c\}$$respectively. Half spaces are convex. A set that can be expressed as the intersection of a finite number of closed half spaces is called a *convex polytope*. A nonempty bounded convex polytope is called a *polyhedron*.





