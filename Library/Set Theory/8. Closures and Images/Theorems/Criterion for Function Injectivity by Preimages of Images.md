**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$.
1. Suppose $S\subseteq A$. Then, $S\subseteq f^{-1}[f[S]]$.
2. $f$ is injective if and only if for all sets $S\subseteq A$, $$S=f^{-1}[f[S]].$$

**Proof of First Statement.** Suppose $x\in S$. Then, $f(x)\in f[S]$, so $x\in f^{-1}[f[S]]$. $\blacksquare$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $f$ is injective. Suppose $S\subseteq A$. By the first statement, we have $S\subseteq f^{-1}[f[S]]$. Now suppose $x\in f^{-1}[f[S]]$. Then, $f(x)\in f(S)$, so there is $y\in S$ such that $f(x)=f(y)$. Since $f$ is injective, we must have $x=y$, so $x\in S$.
- **Backward Implication.** Suppose that for all sets $S\subseteq A$, $$S=f^{-1}[f[S]].$$Suppose $x,y\in A$, and suppose that $f(x)=f(y)$. Since $x\in A$, by [[Criterion for Singleton Sets as Members of Power Sets]] $\{x\}\subseteq A$, so by assumption $$\{x\}=f^{-1}[f[\{x\}]].$$Since $f(x)=f(y)$ and $f(x)\in f[\{x\}]$, we must have $f(y)\in f[\{x\}]$, so $y\in f^{-1}[f[\{x\}]]$. This means $y\in\{x\}$, so $y=x$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Function]]
- [[Injective Function]]
- [[Image of Subset]]
- [[Preimage of Subset]]

Theorems used:
- [[Criterion for Singleton Sets as Members of Power Sets]]