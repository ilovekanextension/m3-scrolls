**Theorem.** Let $M=(M,\circ)$ and $N=(N,+)$ be monoids. Let $\phi:M\to N$ be a monoid homomorphism. Then, $\text{im}(\phi)$ is a submonoid of $S$.

**Proof.**
- **Closure Under Identity.** Since $\phi(1_{M})=1_{N}$, by definition $1_{N}\in \text{im}(\phi)$.
- **Closure Under Composition.** Suppose $a,b\in \text{im}(\phi)$. Then, there are $x,y\in M$ such that $\phi(x)=a$ and $\phi(y)=b$. We then have $$a+b=\phi(x)+\phi(y)=\phi(x\circ y),$$so $a\circ b\in \text{im}(\phi)$. $\blacksquare$

***
Definitions used:
- [[Monoid]]
- [[Monoid Homomorphism]]
- [[Submonoid]]
- [[Image of Function]]