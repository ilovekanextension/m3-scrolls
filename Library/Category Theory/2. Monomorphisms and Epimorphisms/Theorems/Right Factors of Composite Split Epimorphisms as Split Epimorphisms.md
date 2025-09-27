**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be morphisms in $\mathsf{C}$. Suppose that $g\circ f$ is a split epimorphism. Then, $g$ is a split epimorphism.

**Proof.** Since $g\circ f$ is a split epimorphism, there is a morphism $h:C\to A$ such that $(g\circ f)\circ h=\text{id}_{C}$. By associativity, this means $$g\circ(f\circ h)=\text{id}_{C},$$so $g$ is a split epimorphism. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Split Epimorphism]]