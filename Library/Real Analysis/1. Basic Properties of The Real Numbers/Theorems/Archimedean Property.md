**Theorem.**
1. Let $x\in \mathbb{R}$. Then, there is $n\in \mathbb{N}$ such that $x<n$.
2. Let $\varepsilon>0$. Then, there is $n\in \mathbb{N}-\{0\}$ such that $1/n<\varepsilon$.

**Proof of First Statement.** For the sake of contradiction, assume that for all $n\in \mathbb{N}$ we have $\neg(x<n)$. Then, by trichotomy of $<$, for all $n\in \mathbb{N}$ we have $n\leq x$. This means $x$ is an upper bound for $\mathbb{N}$, which contradicts [[Unboundedness of Natural Numbers]]. $\blacksquare$

**Proof of Second Statement.** Since $\varepsilon>0$, by [[Orders Between Additive and Multiplicative Inverses]] $1/\varepsilon>0$. By the first statement, there is $n\in \mathbb{N}$ such that $1/\varepsilon<n$. Since $\varepsilon>0$, $$1=(1/\varepsilon) \cdot\varepsilon<n\cdot\varepsilon.$$Also, since $1/\varepsilon>0$ and $n>1/\varepsilon$, by transitivity $n>0$, so $1/n>0$. Thus, $$1/n=1\cdot(1/n)<n\cdot\varepsilon \cdot(1/n)=\varepsilon.\blacksquare$$
***
Definitions used:
- [[Real Numbers]]
- [[Natural Numbers]]

Theorems used:
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Unboundedness of Natural Numbers]]