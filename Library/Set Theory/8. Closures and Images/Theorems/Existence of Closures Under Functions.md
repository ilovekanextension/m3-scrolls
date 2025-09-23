**Theorem.** Let $A$ be a set. Let $f:A\to A$. Suppose $B\subseteq A$. Define $$S=\{X\subseteq A\mid B\subseteq X\wedge \forall x\in X \ (f(x)\in X)\}.$$Then, $\bigcap S\in S$. Moreover, $\bigcap S$ is the closure of $B$ under $f$. 

**Proof.** We first prove that $\bigcap S\in S$.
- Suppose $b\in B$. Suppose $X\in S$. Then, by definition of $S$, we have $B\subseteq X$. Since $b\in B$, $b\in X$. This shows that $B\subseteq \bigcap S$.
- Suppose $x\in\bigcap S$. Suppose $X\in S$. Then, $x\in X$. Since $X\in S$, we must have $f(x)\in X$. This shows that $\forall x\in\bigcap S \ (f(x)\in\bigcap S)$.

Since $\bigcap S\in S$, by [[Family Intersections and Unions as Smallest and Greatest Objects Under Subset Relation]] $\bigcap S$ is the smallest object of $S$ under $\subseteq$, so for all $X\in S$ we have $\bigcap S\subseteq X$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Intersection of Family of Sets]]
- [[Function]]
- [[Closure of Subset]]
- [[Smallest Object]]

Theorems used:
- [[Family Intersections and Unions as Smallest and Greatest Objects Under Subset Relation]]