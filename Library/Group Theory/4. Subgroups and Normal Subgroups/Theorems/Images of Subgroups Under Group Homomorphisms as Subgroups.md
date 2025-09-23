**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism. Suppose $S$ is a subgroup of $G$. Then, $\phi[S]$ is a subgroup of $H$.

**Proof.**
- **Closure Under Identity.** We have $\phi(1_{G})=1_{H}$. Since $S$ is a subgroup, $1_{G}\in S$, so $1_{H}=\phi(1_{G})\in \phi[S]$.
- **Closure Under Composition.** Suppose $a,b\in \phi[S]$. Then, there is $x,y\in S$ such that $a=\phi(x)$ and $b=\phi(y)$. We then have $$a+b=\phi(x)+\phi(y)=\phi(x\circ y)\in \phi[S].$$
- **Closure Under Inverses.** Suppose $a\in \phi[S]$. Then, there is $x\in S$ such that $a=\phi(x)$. We then have $$a^{-1}=\phi(x)^{-1}=\phi(x^{-1})\in \phi[S].\blacksquare$$

***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Image of Subset]]