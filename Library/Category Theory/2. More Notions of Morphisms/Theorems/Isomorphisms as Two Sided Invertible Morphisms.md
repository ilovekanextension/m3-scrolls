**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ be a morphism in $\mathsf{C}$. Then, $f$ is an isomorphism if and only if $f$ is both a split monomorphism and a split epimorphism.

**Proof of Forward Implication.** Suppose $f$ is an isomorphism. Then, there is $f^{-1}:b\to a$ such that $f^{-1}\circ f=\text{id}_{a}$ and $f\circ f^{-1}=\text{id}_{b}$. The first equality shows that $f$ is a split monomorphism, and the second shows that $f$ is a split epimorphism. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is a split monomorphism and a split epimorphism. Since $f$ is a split monomorphism, there is $g:b\to a$ such that $g\circ f=\text{id}_{a}$. Since $f$ is a split epimorphism, there is $h:b\to a$ such that $f\circ h=\text{id}_{b}$. Observe that $$g=g\circ \text{id}_{b}=g\circ(f\circ h)=(g\circ f)\circ h=\text{id}_{a}\circ h=h.$$Therefore, $g\circ f=\text{id}_{a}$ and $f\circ g=\text{id}_{b}$, so $f$ is an isomorphism with inverse $g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Split Monomorphism]]
- [[Split Epimorphism]]