**Definition.** Let $R$ and $S$ be rings. A function $\phi:R\to S$ is called a **ring homomorphism** if
- $\phi$ is a group homomorphism from $(R,+)$ to $(S,+)$ and
- $\phi$ is a monoid homomorphism from $(R,\cdot)$ to $(S,\cdot)$.

By [[Preservation of Group Identities Under Group Homomorphisms]] and [[Preservation of Group Inverses Under Group Homomorphisms]], in order for $\phi:R\to S$ to be a ring homomorphism, it is therefore enough for $\phi$ to satisfy the following properties.
1. **Preservation of Additions.** For all $a,b\in R$, $$\phi(a+b)=\phi(a)+\phi(b).$$
2. **Preservation of Multiplications.** For all $a,b\in R$, $$\phi(a\cdot b)=\phi(a)\cdot \phi(b).$$
3. **Preservation of Multiplicative Identities.** We have $$\phi(1_{R})=1_{S}.$$

***
Definitions used:
- [[Ring]]
- [[Function]]
- [[Group Homomorphism]]
- [[Monoid Homomorphism]]

Theorems used:
- [[Preservation of Group Identities Under Group Homomorphisms]]
- [[Preservation of Group Inverses Under Group Homomorphisms]]