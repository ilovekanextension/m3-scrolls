**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$.
1. Suppose $T\subseteq B$. Then, $f[f^{-1}[T]]\subseteq T$.
2. $f$ is surjective if and only if for all sets $T\subseteq B$, $$f[f^{-1}[T]]=T.$$

**Proof of First Statement.** Suppose $y\in f[f^{-1}[T]]$. Then, there is $x\in f^{-1}[T]$ such that $y=f(x)$. Since $x\in f^{-1}[T]$, we have $f(x)\in T$, so $y\in T$.

**Proof of Second Statement.**
- **Forward Implication.** Suppose $f$ is surjective. Suppose $T\subseteq B$. By the first statement, $f[f^{-1}[T]]\subseteq T$. Now suppose $y\in T$. Since $f$ is surjective, there is $x\in A$ such that $f(x)=y$. This means $f(x)\in T$, so $x\in f^{-1}[T]$. Therefore, $y=f(x)\in f[f^{-1}[T]]$.
- **Backward Implication.** Suppose that for all sets $T\subseteq B$, $$f[f^{-1}[T]]=T.$$By [[Subset Relation as Partial Order]], $B\subseteq B$, so in particular $f[f^{-1}[B]]=B$. Now suppose $y\in B$. Then, $y\in f[f^{-1}[B]]$, so there is $x\in f^{-1}[B]$ such that $y=f(x)$. By definition, $f^{-1}[B]\subseteq A$, so $x\in A$. Therefore, $f$ is surjective. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Surjective Function]]
- [[Image of Subset]]
- [[Preimage of Subset]]

Theorems used:
- [[Subset Relation as Partial Order]]