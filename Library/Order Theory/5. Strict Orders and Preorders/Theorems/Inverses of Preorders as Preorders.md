**Theorem.** Let $A$ be a set. Let $\leq$ be a preorder on $A$. Let $\geq$ be the inverse of $\leq$. Then, $\geq$ is also a preorder on $A$.

**Proof.**
- **Reflexivity.** Suppose $a\in A$. Since $\leq$ is a partial order, it is reflexive, so $a\leq a$. Therefore, $a\geq a$.
- **Transitivity.** Suppose $a,b,c\in A$, and suppose that $a\geq b$ and $b\geq c$. Then, $b\leq a$ and $c\leq b$. Since $\leq$ is a partial order, it is transitive, so $c\leq a$, which means $a\geq c$. $\blacksquare$

***
Definitions used:
- [[Preorder]]
- [[Set]]
- [[Relation]]
- [[Inverse of Relation]]