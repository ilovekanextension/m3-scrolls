**Theorem.** Let $G$ be a group. Let $S$ be a subgroup of $G$. Suppose $g\in G$.
1. The function $f:S\to g\circ S$ defined as $$f(s)=g\circ s$$is a bijection.
2. The function $f:S\to S\circ g$ defined as $$f(s)=s\circ g$$is a bijection.
3. $g\circ S\cong S\circ g$.

**Proof of First Statement.**
- **Injectivity.** Suppose $s,t\in S$, and suppose that $f(s)=f(t)$. Then, $g\circ s=g\circ t$. By [[Cancellation Properties on Groups]], this means $s=t$.
- **Surjectivity.** Suppose $t\in g\circ S$. Then, there is $s\in S$ such that $t=g\circ s$. Therefore, $t=f(s)$. $\blacksquare$

**Proof of Second Statement.**
- **Injectivity.** Suppose $s,t\in S$, and suppose that $f(s)=f(t)$. Then, $s\circ g=t\circ g$. By [[Cancellation Properties on Groups]], this means $s=t$.
- **Surjectivity.** Suppose $t\in S\circ g$. Then, there is $s\in S$ such that $t=s\circ g$. Therefore, $t=f(s)$. $\blacksquare$

**Proof of Third Statement.** By the first and second statement, $S\cong g\circ S$ and $S\cong S\circ g$. Therefore, by [[Symmetry of Set Isomorphism Relation]] and [[Transitivity of Set Isomorphism Relation]], $g\circ S\cong S\circ g$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Injective Function]]
- [[Surjective Function]]
- [[Bijective Function]]

Theorems used:
- [[Cancellation Properties on Groups]]
- [[Symmetry of Set Isomorphism Relation]]
- [[Transitivity of Set Isomorphism Relation]]