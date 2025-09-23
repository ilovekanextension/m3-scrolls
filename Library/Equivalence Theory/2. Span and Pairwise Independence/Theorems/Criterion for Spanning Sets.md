**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$. Suppose $B\subseteq A$. Then, $B$ spans $A$ if and only if the function $f:B\to A/{\sim}$ defined as $$f(b)=[b]_{\sim}$$is surjective.

**Proof of Forward Implication.** Suppose $B$ spans $A$. Suppose $X\in A/{\sim}$. Then, there is $a\in A$ such that $X=[a]_{\sim}$. Since $B$ spans $A$ and $a\in A$, there is $b\in B$ such that $a\sim b$. By [[Properties of Membership and Equality of Equivalence Classes]], $[a]_{\sim}=[b]_{\sim}$, so $X=[b]_{\sim}$. We then have $f(b)=[b]_{\sim}=X$. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is surjective. Suppose $a\in A$. Then, $[a]_{\sim}\in A/{\sim}$. Since $f$ is surjective, there is $b\in B$ such that $f(b)=[a]_{\sim}$. By definition of $f$, $[b]_{\sim}=[a]_{\sim}$, so by [[Properties of Membership and Equality of Equivalence Classes]] $a\sim b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Spanning Set]]
- [[Function]]
- [[Surjective Function]]

Theorems used:
- [[Properties of Membership and Equality of Equivalence Classes]]