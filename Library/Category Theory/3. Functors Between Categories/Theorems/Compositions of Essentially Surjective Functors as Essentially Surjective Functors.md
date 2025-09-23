**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$ be essentially surjective. Then, $G\circ F$ is essentially surjective.

**Proof.** Suppose $c$ is an object in $\mathsf{E}$. Since $G$ is essentially surjective, there is an object $b$ in $\mathsf{D}$ such that $G(b)\cong c$. Since $F$ is essentially surjective, there is an object $a$ in $\mathsf{C}$ such that $F(a)\cong b$. By [[Preservation of Isomorphisms Under Functors]], we then have $G(F(a))\cong G(b)$. Since $G(b)\cong c$, by [[Isomorphism Relation as Equivalence Relation]] we have $G(F(a))\cong c$, so $G\circ F(a)\cong c$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Essentially Surjective Functor]]

Theorems used:
- [[Isomorphism Relation as Equivalence Relation]]
- [[Preservation of Isomorphisms Under Functors]]