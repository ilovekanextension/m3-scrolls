**Theorem.** Let $A$ be a set. Let $\leq$ be a total order on $A$. Let $\geq$ be the inverse of $\leq$. Then, $\geq$ is also a total order on $A$.

**Proof.** Since $\leq$ is a total order, it is a partial order, so by [[Inverses of Partial Orders as Partial Orders]] $\geq$ is also a partial order. We now show that $\geq$ is connected.

Suppose $a,b\in A$. Since $\leq$ is a total order, $a\leq b$ or $b\leq a$, so $b\geq a$ or $a\geq b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Inverse of Relation]]
- [[Partial Order]]
- [[Total Order]]

Theorems used:
- [[Inverses of Partial Orders as Partial Orders]]