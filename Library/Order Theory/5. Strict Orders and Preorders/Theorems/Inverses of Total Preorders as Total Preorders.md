**Theorem.** Let $A$ be a set. Let $\leq$ be a total preorder on $A$. Let $\geq$ be the inverse of $\leq$. Then, $\geq$ is also a total preorder on $A$.

**Proof.** Since $\leq$ is a total preorder, it is a preorder, so by [[Inverses of Preorders as Preorders]] $\geq$ is also a preorder. We will show that $\geq$ is connected.

Suppose $a,b\in A$. Since $\leq$ is a total preorder, $a\leq b$ or $b\leq a$. Therefore, $b\geq a$ or $a\geq b$. $\blacksquare$
***
Definitions used:
- [[Preorder]]
- [[Total Preorder]]
- [[Set]]
- [[Relation]]
- [[Inverse of Relation]]

Theorems used:
- [[Inverses of Preorders as Preorders]]