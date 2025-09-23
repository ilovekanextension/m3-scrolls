**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ be full and faithful. Then, $F$ is also essentially injective in the following sense:
- For all objects $a$ and $b$ in $\mathsf{C}$, if $F(a)\cong F(b)$, then $a\cong b$.

**Proof.** Suppose $a$ and $b$ are objects in $\mathsf{C}$, and suppose that $F(a)\cong F(b)$. Then, by definition there is an isomorphism $g:F(a)\to F(b)$. Since $F$ is full, there is $f:a\to b$ in $\mathsf{C}$ such that $F(f)=g$. Since $F$ is full and faithful, by [[Reflection of Isomorphisms Under Full and Faithful Functors]], $f$ is an isomorphism, so $a\cong b$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Faithful Functor]]
- [[Full Functor]]

Theorems used:
- [[Reflection of Isomorphisms Under Full and Faithful Functors]]