**Theorem.** Let $A$ be a set.
1. The subset relation $\subseteq$ is a partial order on $\mathcal{P}(A)$.
2. Suppose $F$ is a family of subsets of $A$, and suppose that $\bigcap F\in F$. Then, $\bigcap F$ is the smallest object of $F$ under $\subseteq$.
3. Suppose $F$ is a family of subsets of $A$, and suppose that $\bigcup F\in F$. Then, $\bigcup F$ is the greatest object of $F$ under $\subseteq$.

**Proof of First Statement.** By [[Subset Relation as Partial Order]], $\subseteq$ is reflexive and transitive. Antisymmetry holds by definition. $\blacksquare$

**Proof of Second Statement.** Suppose $A\in F$. Suppose $x\in\bigcap F$. Then, for all $X\in F$ we have $x\in X$. Since $A\in F$, we therefore have $x\in A$. $\blacksquare$

**Proof of Third Statement.** Suppose $A\in F$. Suppose $x\in A$. Then, there is $X\in F$ such that $x\in X$. Therefore, $x\in\bigcup F$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Power Set]]
- [[Union of Family of Sets]]
- [[Intersection of Family of Sets]]
- [[Partial Order]]
- [[Smallest Object]]
- [[Greatest Object]]

Theorems used:
- [[Subset Relation as Partial Order]]