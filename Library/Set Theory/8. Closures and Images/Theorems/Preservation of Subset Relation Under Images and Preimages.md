**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$.
1. Suppose $T\subseteq A$ and $S\subseteq T$. Then, $f[S]\subseteq f[T]$.
2. Suppose $T\subseteq B$ and $S\subseteq T$. Then, $f^{-1}[S]\subseteq f^{-1}[T]$.

**Proof of First Statement.** Suppose $x\in f[S]$. Then, there is $a\in S$ such that $x=f(a)$. Since $S$ is a subset of $T$, we have $a\in T$, so $x\in f[T]$. $\blacksquare$

**Proof of Second Statement.** Suppose $x\in f^{-1}[S]$. Then, $f(x)\in S$. Since $S$ is a subset of $T$, we have $f(x)\in T$, so $x\in f^{-1}[T]$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Function]]
- [[Image of Subset]]
- [[Preimage of Subset]]