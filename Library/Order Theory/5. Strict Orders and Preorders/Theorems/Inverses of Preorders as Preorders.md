**Theorem.** Let $A$ be a set. Let $\prec$ be a preorder on $A$. Let $\succ$ be the inverse of $\prec$. Then, $\succ$ is also a preorder on $A$.

**Proof.**
- **Reflexivity.** Suppose $a\in A$. Since $\prec$ is a partial order, it is reflexive, so $a\prec a$. Therefore, $a\succ a$.
- **Transitivity.** Suppose $a,b,c\in A$, and suppose that $a\succ b$ and $b\succ c$. Then, $b\prec a$ and $c\prec b$. Since $\prec$ is a partial order, it is transitive, so $c\prec a$, which means $a\succ c$. $\blacksquare$

***
Definitions used:
- [[Preorder]]
- [[Set]]
- [[Relation]]
- [[Inverse of Relation]]