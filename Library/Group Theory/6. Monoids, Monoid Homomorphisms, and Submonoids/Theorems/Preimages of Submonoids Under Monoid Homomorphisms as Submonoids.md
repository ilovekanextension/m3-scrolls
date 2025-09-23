**Theorem.** Let $M=(M,\circ)$ and $N=(N,+)$ be monoids. Let $\phi:M\to N$ be a monoid homomorphism. Suppose $T$ is a submonoid of $N$. Then, $\phi^{-1}[T]$ is a submonoid of $M$.

**Proof.**
- **Closure Under Identity.** Since $T$ is a submonoid, $1_{N}\in T$. We have $\phi(1_{M})=1_{N}\in T$, so $1_{M}\in \phi^{-1}[T]$.
- **Closure Under Composition.** Suppose $x,y\in \phi^{-1}[T]$. Then, $\phi(x)\in T$ and $\phi(y)\in T$. Since $T$ is a submonoid, $\phi(x)+\phi(y)\in T$. This means $$\phi(x\circ y)=\phi(x)+\phi(y)\in T,$$so $x\circ y\in \phi^{-1}[T]$. $\blacksquare$

***
Definitions used:
- [[Monoid]]
- [[Monoid Homomorphism]]
- [[Submonoid]]
- [[Preimage of Subset]]