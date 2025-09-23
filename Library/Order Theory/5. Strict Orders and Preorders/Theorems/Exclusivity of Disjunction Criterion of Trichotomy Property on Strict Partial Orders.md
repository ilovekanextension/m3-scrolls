**Theorem.** Let $A$ be a set. Let $<$ be a strict partial order on $A$. Suppose that for all $a,b\in A$, we have $$(a<b)\vee(b<a)\vee(a=b).$$Then, for all $a,b\in A$, only one of the conditions above can be true. That is, the condition above can be made stronger as follows: for all $a,b\in A$, exactly one of the following holds:
- $a<b$.
- $b<a$.
- $a=b$.

**Proof.** Suppose $a,b\in A$. By assumption, at least one of the three conditions holds.

First suppose that $a<b$. To show that $\neg(b<a)$, assume for the sake of negation that $b<a$. Then, since $<$ is a strict partial order, $<$ is assymetric, so $\neg(a<b)$, which contradicts the supposition $a<b$. To show that $a\neq b$, assume for the sake of negation that $a=b$. Then, since $a<b$, we have $a<a$. Since $<$ is a strict partial order, $<$ is irreflexive, so $\neg(a<a)$, which gives a contradiction.

By a similar reasoning, we can conclude that if $b<a$, then $\neg(a<b)$ and $a\neq b$.

Finally, suppose that $a=b$. To show that $\neg(a<b)$, assume for the sake of negation that $a<b$. Then, since $a=b$, we have $a<a$. Since $<$ is a strict partial order, $<$ is irreflexive, so $\neg(a<a)$, which gives a contradiction. By a similar reasoning, we also have $\neg(b<a)$. $\blacksquare$
***
Definitions used:
- [[Strict Partial Order]]
- [[Set]]
- [[Relation]]