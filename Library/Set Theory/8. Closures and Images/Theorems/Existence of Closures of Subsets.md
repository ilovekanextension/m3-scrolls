**Theorem.** Let $A$ be a set.
1. Let $f:A\to A$. Suppose $B\subseteq A$. Define $$S=\{X\subseteq A\mid B\subseteq X\wedge \forall x\in X \ (f(x)\in X)\}.$$Then, $\bigcap S\in S$. Moreover, $\bigcap S$ is the closure of $B$ under $f$.
2. Let $\circ:A\times A\to A$. Suppose $B\subseteq A$. Define $$S=\{X\subseteq A\mid B\subseteq X\wedge \forall x,y\in X \ (x\circ y\in X)\}.$$Then, $\bigcap S\in S$. Moreover, $\bigcap S$ is the closure of $B$ under $\circ$.

**Proof of First Statement.** We first prove that $\bigcap S\in S$.
- To show that $B\subseteq \bigcap S$, suppose $b\in B$, and suppose that $X\in S$. Then, by definition of $S$, we have $B\subseteq X$. Since $b\in B$, we have $b\in X$.
- To show that for all $x\in\bigcap S$ we have $f(x)\in\bigcap S$, suppose $x\in\bigcap S$, and suppose that $X\in S$. Then, $x\in X$. Since $X\in S$, we must have $f(x)\in X$.

Since $\bigcap S\in S$, by [[Family Intersections and Unions as Smallest and Greatest Objects Under Subset Relation]] $\bigcap S$ is the smallest object of $S$ under $\subseteq$, so for all $X\in S$ we have $\bigcap S\subseteq X$. $\blacksquare$

**Proof of Second Statement.** We first prove that $\bigcap S\in S$.
- To show that $B\subseteq \bigcap S$, suppose $b\in B$, and suppose that $X\in S$. Then, by definition of $S$, we have $B\subseteq X$. Since $b\in B$, we have $b\in X$.
- To show that for all $x,y\in\bigcap S$ we have $x\circ y\in\bigcap S$, suppose $x,y\in\bigcap S$, and suppose that $X\in S$. Then, $x,y\in X$. Since $X\in S$, we must have $x\circ y\in X$.

Since $\bigcap S\in S$, by [[Family Intersections and Unions as Smallest and Greatest Objects Under Subset Relation]] $\bigcap S$ is the smallest object of $S$ under $\subseteq$, so for all $X\in S$ we have $\bigcap S\subseteq X$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Intersection of Family of Sets]]
- [[Function]]
- [[Closed Subset]]
- [[Closure of Subset]]
- [[Smallest Object]]

Theorems used:
- [[Family Intersections and Unions as Smallest and Greatest Objects Under Subset Relation]]