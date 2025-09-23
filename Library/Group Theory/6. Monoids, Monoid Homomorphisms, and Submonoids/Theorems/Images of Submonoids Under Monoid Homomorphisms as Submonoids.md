**Theorem.** Let $M=(M,\circ)$ and $N=(N,+)$ be monoids. Let $\phi:M\to N$ be a monoid homomorphism. Suppose $S$ is a submonoid of $M$. Then, $\phi[S]$ is a submonoid of $N$.

**Proof.**
- **Closure Under Identity.** Since $S$ is a submonoid, $1_{M}\in S$. Therefore, $1_{N}=\phi(1_{M})\in \phi[S]$.
- **Closure Under Composition.** Suppose $a,b\in \phi[S]$. Then, there are $x,y\in S$ such that $\phi(x)=a$ and $\phi(y)=b$. Since $S$ is a submonoid, $x\circ y\in S$, so $$a+b=\phi(x)+\phi(y)=\phi(x\circ y)\in \phi[S].\blacksquare$$

***
Definitions used:
- [[Monoid]]
- [[Monoid Homomorphism]]
- [[Submonoid]]
- [[Image of Subset]]