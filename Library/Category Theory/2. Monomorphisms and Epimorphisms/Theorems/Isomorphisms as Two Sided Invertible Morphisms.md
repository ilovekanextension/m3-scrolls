**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a morphism in $\mathsf{C}$. Then, $f$ is an isomorphism if and only if $f$ is both a split monomorphism and a split epimorphism.

**Proof of Forward Implication.** Suppose $f$ is an isomorphism. Then, there is $f^{-1}:B\to A$ such that $f^{-1}\circ f=\text{id}_{A}$ and $f\circ f^{-1}=\text{id}_{B}$. The first equality shows that $f$ is a split monomorphism, and the second shows that $f$ is a split epimorphism. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is a split monomorphism and a split epimorphism. Since $f$ is a split monomorphism, there is $g:B\to A$ such that $g\circ f=\text{id}_{A}$. Since $f$ is a split epimorphism, there is $h:B\to A$ such that $f\circ h=\text{id}_{B}$. Observe that $$g=g\circ \text{id}_{B}=g\circ(f\circ h)=(g\circ f)\circ h=\text{id}_{A}\circ h=h.$$Therefore, $g\circ f=\text{id}_{A}$ and $f\circ g=\text{id}_{B}$, so $f$ is an isomorphism with inverse $g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Split Monomorphism]]
- [[Split Epimorphism]]