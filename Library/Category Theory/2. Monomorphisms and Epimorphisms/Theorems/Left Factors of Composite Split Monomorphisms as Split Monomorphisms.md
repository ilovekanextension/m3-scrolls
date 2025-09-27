**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be morphisms in $\mathsf{C}$. Suppose that $g\circ f$ is a split monomorphism. Then, $f$ is a split monomorphism.

**Proof.** Since $g\circ f$ is a split monomorphism, there is a morphism $h:C\to A$ such that $h\circ(g\circ f)=\text{id}_{A}$. By associativity, this means $$(h\circ g)\circ f=\text{id}_{A},$$so $f$ is a split monomorphism. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Split Monomorphism]]