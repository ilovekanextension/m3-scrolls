**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ be full and faithful. Then, $F$ is also essentially injective in the following sense:
- For all objects $A$ and $B$ in $\mathsf{C}$, if $F(A)\cong F(B)$, then $A\cong B$.

**Proof.** Suppose $A$ and $B$ are objects in $\mathsf{C}$, and suppose that $F(A)\cong F(B)$. Then, by definition there is an isomorphism $g:F(A)\to F(B)$. Since $F$ is full, there is $f:A\to B$ in $\mathsf{C}$ such that $F(f)=g$. Since $F$ is full and faithful, by [[Reflection of Isomorphisms Under Full and Faithful Functors]], $f$ is an isomorphism, so $A\cong B$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Faithful Functor]]
- [[Full Functor]]

Theorems used:
- [[Reflection of Isomorphisms Under Full and Faithful Functors]]