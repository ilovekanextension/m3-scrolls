**Theorem.** Let $\mathsf{C}$ be a category.
1. For all objects $A$ in $\mathsf{C}$, $A\cong A$.
2. For all objects $A$ and $B$ in $\mathsf{C}$, if $A\cong B$, then $B\cong A$.
3. For all objects $A$, $B$, and $C$ in $\mathsf{C}$, if $A\cong B$ and $B\cong C$, then $A\cong C$.

**Proof of First Statement.** Suppose $A$ is an object in $\mathsf{C}$. By [[Identity Morphisms as Isomorphisms]], $\text{id}_{A}:A\to A$ is an isomorphism, so $A\cong A$. $\blacksquare$

**Proof of Second Statement.** Suppose $A$ and $B$ are objects in $\mathsf{C}$. Suppose $A\cong B$. Then, there is an isomorphism $f:A\to B$. By [[Inverses of Isomorphisms as Isomorphisms]], $f^{-1}:B\to A$ is also an isomorphism, so $B\cong A$. $\blacksquare$

**Proof of Third Statement.** Suppose $A$, $B$, and $C$ are objects in $\mathsf{C}$. Suppose $A\cong B$ and $B\cong C$. Then, there are isomorphisms $f:A\to B$ and $g:B\to C$. By [[Compositions of Isomorphisms as Isomorphisms]], $g\circ f:A\to C$ is also an isomorphism, so $A\cong C$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]

Theorems used:
- [[Identity Morphisms as Isomorphisms]]
- [[Inverses of Isomorphisms as Isomorphisms]]
- [[Compositions of Isomorphisms as Isomorphisms]]