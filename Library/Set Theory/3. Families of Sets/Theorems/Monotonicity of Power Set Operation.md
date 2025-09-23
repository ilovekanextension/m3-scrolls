**Theorem.** Let $A$ and $B$ be sets. Then, $A\subseteq B$ if and only if $\mathcal{P}(A)\subseteq\mathcal{P}(B)$.

**Proof of Forward Implication.** Suppose $A\subseteq B$. Suppose $x\in\mathcal{P}(A)$. Then, $x\subseteq A$. Since $A\subseteq B$, by [[Subset Relation as Partial Order]] we have $x\subseteq B$, so $x\in\mathcal{P}(B)$. $\blacksquare$

**Proof of Backward Implication.** Suppose $\mathcal{P}(A)\subseteq \mathcal{P}(B)$. Suppose $x\in A$. Then, by [[Criterion for Singleton Sets as Members of Power Sets]], $\{x\}\subseteq A$, so $\{x\}\in\mathcal{P}(A)$. Since $\mathcal{P}(A)\subseteq \mathcal{P}(B)$, we have $\{x\}\in\mathcal{P}(B)$, so $\{x\}\subseteq B$. Since $x\in\{x\}$, we have $x\in B$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Enumeration Notation]]
- [[Power Set]]

Theorems used:
- [[Subset Relation as Partial Order]]
- [[Criterion for Singleton Sets as Members of Power Sets]]