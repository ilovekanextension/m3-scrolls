**Theorem.** Let $A$ be a set. Let $<$ be a relation on $A$ satisfying the following properties.
- **Irreflexivity.** For all $a\in A$, $\neg(a<a)$.
- **Transitivity.** For all $a,b,c\in A$, if $a<b$ and $b<c$, then $a<c$.

Then, for all $a,b\in A$, if $a<b$, then $\neg(b<a)$.

**Proof.** Suppose $a,b\in A$, and suppose that $a<b$. Assume for the sake of negation that $b<a$. Then, by transitivity $a<a$. This contradicts the fact that $\neg(a<a)$ by irreflexivity. Therefore, the assumption that $b<a$ is false, so $\neg(b<a)$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Relation]]