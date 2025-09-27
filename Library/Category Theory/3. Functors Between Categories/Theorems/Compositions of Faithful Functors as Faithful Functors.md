**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$ be faithful. Then, $G\circ F$ is faithful.

**Proof.** Suppose $A$ and $B$ are objects in $\mathsf{C}$. Suppose $f:A\to B$ and $g:A\to B$ are morphisms in $\mathsf{C}$, and suppose that $$G\circ F(f)=G\circ F(g).$$Then, $G(F(f))=G(F(g))$. Since $G$ is faithful, we have $F(f)=F(g)$. Since $F$ is faithful, we have $f=g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Composition of Functors]]
- [[Faithful Functor]]