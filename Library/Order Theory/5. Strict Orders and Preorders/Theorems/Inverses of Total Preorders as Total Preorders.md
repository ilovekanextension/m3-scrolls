**Theorem.** Let $A$ be a set. Let $\prec$ be a total preorder on $A$. Let $\succ$ be the inverse of $\prec$. Then, $\succ$ is also a total preorder on $A$.

**Proof.** Since $\prec$ is a total preorder, it is a preorder, so by [[Inverses of Preorders as Preorders]] $\succ$ is also a preorder. We will show that $\succ$ is connected.

Suppose $a,b\in A$. Since $\prec$ is a total preorder, $a\prec b$ or $b\prec a$. Therefore, $b\succ a$ or $a\succ b$. $\blacksquare$
***
Definitions used:
- [[Preorder]]
- [[Total Preorder]]
- [[Set]]
- [[Relation]]
- [[Inverse of Relation]]

Theorems used:
- [[Inverses of Preorders as Preorders]]