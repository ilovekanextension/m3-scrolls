**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ be full and faithful. Suppose $f:a\to b$ is a morphism in $\mathsf{C}$, and suppose that $F(f)$ is an isomorphism. Then, $f$ is also an isomorphism.

**Proof.** Since $F(f)$ is an isomorphism, there is a morphism $F(f)^{-1}:F(b)\to F(a)$ such that $F(f)^{-1}\circ F(f)=\text{id}_{F(a)}$ and $F(f)\circ F(f)^{-1}=\text{id}_{F(b)}$. Since $F$ is full, there is a morphism $g:b\to a$ in $\mathsf{C}$ such that $F(g)=F(f)^{-1}$. Since $F$ is a functor, we have $$F(g\circ f)=F(g)\circ F(f)=F(f)^{-1}\circ F(f)=\text{id}_{F(a)}=F(\text{id}_{a})$$and $$F(f\circ g)=F(f)\circ F(g)=F(f)\circ F(f)^{-1}=\text{id}_{F(b)}=F(\text{id}_{b}).$$Since $F$ is faithful, from these equalities we have $g\circ f=\text{id}_{a}$ and $f\circ g=\text{id}_{b}$, so $f$ is an isomorphism with inverse $g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Faithful Functor]]
- [[Full Functor]]