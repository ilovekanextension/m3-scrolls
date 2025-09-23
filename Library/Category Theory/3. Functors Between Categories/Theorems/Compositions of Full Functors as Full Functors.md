**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$ be full. Then, $G\circ F$ is full.

**Proof.** Suppose $a$ and $b$ are objects in $\mathsf{C}$. Suppose $h:G\circ F(a)\to G\circ F(b)$ is a morphism in $\mathsf{E}$. Then, we have $h:G(F(a))\to G(F(b))$. Since $G$ is full, there is $g:F(a)\to F(b)$ in $\mathsf{D}$ such that $G(g)=h$. Since $F$ is full, there is $f:a\to b$ in $\mathsf{C}$ such that $F(f)=g$. We then have $G(F(f))=h$, so $G\circ F(f)=h$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Composition of Functors]]
- [[Full Functor]]