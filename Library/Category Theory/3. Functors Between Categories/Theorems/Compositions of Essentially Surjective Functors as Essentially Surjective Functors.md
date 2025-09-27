**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$ be essentially surjective. Then, $G\circ F$ is essentially surjective.

**Proof.** Suppose $C$ is an object in $\mathsf{E}$. Since $G$ is essentially surjective, there is an object $B$ in $\mathsf{D}$ such that $G(B)\cong C$. Since $F$ is essentially surjective, there is an object $A$ in $\mathsf{C}$ such that $F(A)\cong B$. By [[Preservation of Isomorphisms Under Functors]], we then have $G(F(A))\cong G(B)$. Since $G(B)\cong C$, by [[Isomorphism Relation as Equivalence Relation]] we have $G(F(A))\cong C$, so $G\circ F(A)\cong C$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Essentially Surjective Functor]]

Theorems used:
- [[Isomorphism Relation as Equivalence Relation]]
- [[Preservation of Isomorphisms Under Functors]]