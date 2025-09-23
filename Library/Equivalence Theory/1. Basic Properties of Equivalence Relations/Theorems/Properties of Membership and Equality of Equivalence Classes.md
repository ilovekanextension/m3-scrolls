**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$.
1. Suppose $a\in A$. Then, $a\in[a]_{\sim}$.
2. Suppose $a,b\in A$. Then, $a\sim b$ if and only if $[a]_{\sim}=[b]_{\sim}$.

**Proof of First Statement.** By reflexivity, $a\sim a$, so $a\in[a]_{\sim}$. $\blacksquare$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $a\sim b$. Suppose $x\in A$. First suppose $x\in[a]_{\sim}$. Then, $x\sim a$. Since $a\sim b$, by transitivity $x\sim b$, so $x\in[b]_{\sim}$. Now suppose $x\in[b]_{\sim}$. Then, $x\sim b$. Since $a\sim b$, by symmetry $b\sim a$, so by transitivity $x\sim a$. This means $x\in[a]_{\sim}$. $\blacksquare$
- **Backward Implication.** Suppose $[a]_{\sim}=[b]_{\sim}$. By the first statement, $a\in[a]_{\sim}$. Since $[a]_{\sim}=[b]_{\sim}$, $a\in[b]_{\sim}$, so $a\sim b$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Equivalence Relation]]
- [[Equivalence Class]]