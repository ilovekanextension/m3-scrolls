**Theorem.** Let $A$ be a set. Let $<$ be a strict partial order on $A$. Let $>$ be the inverse of $<$. Then, $>$ is also a strict partial order on $A$.

**Proof.**
- **Irreflexivity.** Suppose $a\in A$. Since $<$ is a strict partial order, $<$ is irreflexive, so $\neg(a<a)$. Therefore, $\neg(a>a)$.
- **Transitivity.** Suppose $a,b,c\in A$, and suppose that $a>b$ and $b>c$. Then, $b<a$ and $c<b$. Since $<$ is a strict partial order, $<$ is transitive, so $c<a$. This means $a>c$. $\blacksquare$

***
Definitions used:
- [[Strict Partial Order]]
- [[Set]]
- [[Relation]]
- [[Inverse of Relation]]