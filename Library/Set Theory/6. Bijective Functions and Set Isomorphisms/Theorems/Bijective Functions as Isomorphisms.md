**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Then, $f$ is an isomorphism if and only if $f$ is bijective.

**Proof of Forward Implication.** Suppose $f$ is an isomorphism. Then, there is a function $g:B\to A$ such that $g\circ f=\text{id}_{A}$ and $f\circ g=\text{id}_{B}$. By [[Injectivity of Left Invertible Functions]] and [[Surjectivity of Right Invertible Functions]], this means $f$ is injective and surjective, so $f$ is bijective. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is bijective. Then, by [[Relation Inverses of Bijective Functions as Functions]], $f^{-1}:B\to A$. Moreover, by [[Compositions of Bijective Functions with Their Inverses as Identity Functions]], $f^{-1}\circ f=\text{id}_{A}$ and $f\circ f^{-1}=\text{id}_{B}$. This means $f$ is an isomorphism. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Category of Sets]]
- [[Injective Function]]
- [[Surjective Function]]
- [[Bijective Function]]
- [[Isomorphism]]

Theorems used:
- [[Injectivity of Left Invertible Functions]]
- [[Surjectivity of Right Invertible Functions]]
- [[Relation Inverses of Bijective Functions as Functions]]
- [[Compositions of Bijective Functions with Their Inverses as Identity Functions]]