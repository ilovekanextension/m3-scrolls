**Theorem.** Let $G$ be a group. Then, there is a subgroup $S$ of $S_{G}$ such that $G\cong S$.

**Proof.** By [[Group Compositions as Group Actions]], $\circ:G\times G\to G$ is a group action on $G$. Therefore, by [[Group Actions on Sets as Group Homomorphisms]], the function $\sigma:G\to S_{G}$ defined as $$\sigma(g)=\circ(g,-)=g\circ-$$is a group homomorphism. We will show that $G\cong\text{im}(\sigma)$; by [[Images of Group Homomorphisms as Subgroups]], $\text{im}(\sigma)$ is a subgroup of $S_{G}$, so $G$ is isomorphic to a subgroup of $S_{G}$.

Consider the restriction $\sigma:G\to \text{im}(\sigma)$. Clearly this restriction is surjective. We will show that it is also injective. Suppose $g,h\in G$, and suppose that $\sigma(g)=\sigma(h)$. Then, $g\circ-=h\circ-$. By [[Extensionality of Functions]], we then have $$g=g\circ 1=g\circ-(1)=h\circ-(1)=h\circ 1=h.\blacksquare$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Group Isomorphism]]
- [[Symmetric Group]]
- [[Group Action on Set]]
- [[Subgroup]]
- [[Injective Function]]
- [[Image of Function]]

Theorems used:
- [[Group Actions on Sets as Group Homomorphisms]]
- [[Group Compositions as Group Actions]]
- [[Images of Group Homomorphisms as Subgroups]]
- [[Extensionality of Functions]]