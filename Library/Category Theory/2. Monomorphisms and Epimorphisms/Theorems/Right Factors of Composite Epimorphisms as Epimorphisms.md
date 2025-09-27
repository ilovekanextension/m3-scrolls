**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be morphisms in $\mathsf{C}$. Suppose that $g\circ f$ is an epimorphism. Then, $g$ is an epimorphism.

**Proof.** Suppose $s:C\to X$ and $t:C\to X$ are morphisms in $\mathsf{C}$, and suppose that $$s\circ g=t\circ g.$$Then, $(s\circ g)\circ f=(t\circ g)\circ f$, so by associativity $$s\circ(g\circ f)=t\circ(g\circ f).$$Since $g\circ f$ is an epimorphism, we have $s=t$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Epimorphism]]