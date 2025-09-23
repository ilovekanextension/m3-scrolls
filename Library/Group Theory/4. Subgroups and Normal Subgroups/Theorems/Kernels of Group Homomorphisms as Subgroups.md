**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism.
1. $1_{G}\in\ker(\phi)$.
2. For all $a,b\in\ker(\phi)$, $a\circ b\in\ker(\phi)$.
3. For all $a\in\ker(\phi)$, $a^{-1}\in\ker(\phi)$.

Therefore, $\ker(\phi)$ is a subgroup of $G$.

**Proof of First Statement.** Since $\phi(1_{G})=1_{H}$, by definition $1_{G}\in\ker(\phi)$. $\blacksquare$

**Proof of Second Statement.** Suppose $a,b\in\ker(\phi)$. Then, $\phi(a)=1_{H}$ and $\phi(b)=1_{H}$. This means $$\phi(a\circ b)=\phi(a)+\phi(b)=1_{H}+1_{H}=1_{H},$$so $a\circ b\in\ker(\phi)$. $\blacksquare$

**Proof of Third Statement.** Suppose $a\in\ker(\phi)$. Then, $\phi(a)=1_{H}$. By [[Inverses of Group Identities]], $$\phi(a^{-1})=\phi(a)^{-1}=1_{H}^{-1}=1_{H},$$so $a^{-1}\in\ker(\phi)$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Kernel of Group Homomorphism]]

Theorems used:
- [[Inverses of Group Identities]]