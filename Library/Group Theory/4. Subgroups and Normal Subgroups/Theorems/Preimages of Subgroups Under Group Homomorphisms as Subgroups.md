**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism. Suppose $T$ is a subgroup of $H$. Then, $\phi^{-1}[T]$ is a subgroup of $G$.

**Proof.**
- **Closure Under Identity.** We have $\phi(1_{G})=1_{H}$. Since $T$ is a subgroup of $H$, $1_{H}\in T$, so $\phi(1_{G})\in T$. Therefore, $1_{G}\in \phi^{-1}[T]$.
- **Closure Under Composition.** Suppose $a,b\in \phi^{-1}[T]$. Then, $\phi(a)\in T$ and $\phi(b)\in T$. We then have $$\phi(a\circ b)=\phi(a)+\phi(b)\in T,$$so $a\circ b\in \phi^{-1}[T]$.
- **Closure Under Inverses.** Suppose $a\in \phi^{-1}[T]$. Then, $\phi(a)\in T$. We then have $$\phi(a^{-1})=\phi(a)^{-1}\in T,$$so $a^{-1}\in \phi^{-1}[T]$. $\blacksquare$

***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Preimage of Subset]]