**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism.
1. $1_{H}\in \text{im}(\phi)$.
2. For all $g,h\in \text{im}(\phi)$, $g+h\in \text{im}(\phi)$.
3. For all $g\in \text{im}(\phi)$, $g^{-1}\in \text{im}(\phi)$.

Therefore, $\text{im}(\phi)$ is a subgroup of $H$.

**Proof of First Statement.** Since $\phi(1_{G})=1_{H}$, by definition $1_{H}\in \text{im}(\phi)$. $\blacksquare$

**Proof of Second Statement.** Suppose $g,h\in \text{im}(\phi)$. Then, there are $a,b\in G$ such that $g=\phi(a)$ and $h=\phi(b)$. We have $$g+h=\phi(a)+\phi(b)=\phi(a\circ b),$$so $g+h\in \text{im}(\phi)$. $\blacksquare$

**Proof of Third Statement.** Suppose $g\in \text{im}(\phi)$. Then, there is $a\in G$ such that $g=\phi(a)$. We have $$g^{-1}=\phi(a)^{-1}=\phi(a^{-1}),$$so $g^{-1}\in \text{im}(\phi)$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Image of Function]]