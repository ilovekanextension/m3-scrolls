**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $b$ is the greatest object of $B$ under $\leq$.
1. $b$ is a maximal object of $B$ under $\leq$.
2. Suppose $c$ is a maximal object of $B$ under $\leq$. Then, $b=c$.

**Proof.** By [[Duality of Smallest and Greatest Objects]], $b$ is the smallest object of $B$ under $\leq^\text{op}$.
- **First Statement.** By [[Minimality of Smallest Objects]] $b$ is a minimal object of $B$ under $\leq^{\text{op}}$, so by [[Duality of Minimal and Maximal Objects]] $b$ is a maximal object of $B$ under $\leq^{\text{op}}$. $\blacksquare$
- **Second Statement.** By [[Duality of Minimal and Maximal Objects]], $c$ is minimal under $\leq^{\text{op}}$, so by [[Minimality of Smallest Objects]] $b=c$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Partial Order]]
- [[Minimal Object]]
- [[Dual Order]]
- [[Maximal Object]]

Theorems used:
- [[Minimality of Smallest Objects]]
- [[Duality of Smallest and Greatest Objects]]
- [[Duality of Minimal and Maximal Objects]]