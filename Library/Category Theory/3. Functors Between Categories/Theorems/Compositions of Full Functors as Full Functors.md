**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$ be full. Then, $G\circ F$ is full.

**Proof.** Suppose $A$ and $B$ are objects in $\mathsf{C}$. Suppose $h:G\circ F(A)\to G\circ F(B)$ is a morphism in $\mathsf{E}$. Then, by definition of functor composition we have $$h:G(F(A))\to G(F(B)).$$Since $G$ is full, there is $g:F(A)\to F(B)$ in $\mathsf{D}$ such that $G(g)=h$. Since $F$ is full, there is $f:A\to B$ in $\mathsf{C}$ such that $F(f)=g$. We then have $G(F(f))=h$, so $G\circ F(f)=h$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Composition of Functors]]
- [[Full Functor]]