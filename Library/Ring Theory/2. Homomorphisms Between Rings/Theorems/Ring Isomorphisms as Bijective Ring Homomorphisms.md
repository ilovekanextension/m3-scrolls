**Theorem.** Let $R$ and $S$ be rings. Let $\phi:R\to S$ be a ring homomorphism. Then, the following statements are equivalent.
1. There is a ring homomorphism $\eta:S\to R$ such that $\eta\circ\phi=\text{id}_{R}$ and $\phi\circ\eta=\text{id}_{S}$.
2. $\phi$ is bijective.

**Proof of** $1\Rightarrow 2$. Suppose there is a ring homomorphism $\eta:S\to R$ such that $\eta\circ\phi=\text{id}_{R}$ and $\phi\circ\eta=\text{id}_{S}$. Since ring homomorphisms are functions, by [[Bijective Functions as Isomorphisms]] the statement follows immediately.

**Proof of** $2\Rightarrow 1$. Suppose $\phi$ is bijective. By [[Group Isomorphisms as Bijective Group Homomorphisms]], $\phi^{-1}$ is a group homomorphism from $(S,+)$ to $(R,+)$. By [[Monoid Isomorphisms as Bijective Monoid Homomorphisms]], $\phi^{-1}$ is a monoid homomorphism from $(S,\cdot)$ to $(R,\cdot)$. Therefore, $\phi^{-1}$ is a ring homomorphism from $S$ to $R$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Ring Homomorphism]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Group Homomorphism]]
- [[Monoid Homomorphism]]

Theorems used:
- [[Bijective Functions as Isomorphisms]]
- [[Group Isomorphisms as Bijective Group Homomorphisms]]
- [[Monoid Isomorphisms as Bijective Monoid Homomorphisms]]