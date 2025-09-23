**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$. Suppose $B\subseteq A$. Then, $B$ is pairwise independent if and only if the function $f:B\to A/{\sim}$ defined as $$f(b)=[b]_{\sim}$$is injective.

**Proof of Forward Implication.** Suppose $B$ is pairwise independent. Suppose $a,b\in B$, and suppose that $f(a)=f(b)$. Then, by definition of $f$, $[a]_{\sim}=[b]_{\sim}$, so by [[Properties of Membership and Equality of Equivalence Classes]] $a\sim b$. Since $B$ is pairwise independent, $a=b$. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is injective. Suppose $a,b\in B$, and suppose that $a\sim b$. Then, by [[Properties of Membership and Equality of Equivalence Classes]] $[a]_{\sim}=[b]_{\sim}$, so $f(a)=f(b)$. Since $f$ is injective, $a=b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Pairwise Independent Set]]
- [[Function]]
- [[Injective Function]]

Theorems used:
- [[Properties of Membership and Equality of Equivalence Classes]]