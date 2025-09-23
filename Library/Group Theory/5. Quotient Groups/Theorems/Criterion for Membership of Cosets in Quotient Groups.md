**Theorem.** Let $G$ be a group. Let $S$ be a subgroup of $G$. Let $N$ be a normal subgroup of $G$, and suppose that $N\subseteq S$. Then, for all $a\in G$, $a\circ N\in S/N$ if and only if $a\in S$.

**Proof.** Suppose $a\in G$.
- **Forward Implication.** Suppose $a\circ N\in S/N$. Then, there is $b\in S$ such that $a\circ N=b\circ N$. By [[Criterion for Equality of Cosets]], this means $a^{-1}\circ b\in N$. Since $N\subseteq S$, we have $a^{-1}\circ b\in S$. Since $b\in S$, we must also have $a^{-1}\in S$, so by [[Involution Property on Group Inverses]] $a=(a^{-1})^{-1}\in S$.
- **Backward Implication.** Suppose $a\in S$. Then, by definition $a\circ N\in S/N$. $\blacksquare$

***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Normal Subgroup]]
- [[Quotient Group]]

Theorems used:
- [[Involution Property on Group Inverses]]
- [[Criterion for Equality of Cosets]]