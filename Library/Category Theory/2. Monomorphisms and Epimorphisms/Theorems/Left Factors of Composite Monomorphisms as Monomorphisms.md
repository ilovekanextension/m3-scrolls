**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be morphisms in $\mathsf{C}$. Suppose that $g\circ f$ is a monomorphism. Then, $f$ is a monomorphism.

**Proof.** Suppose $s:X\to A$ and $t:X\to A$ are morphisms in $\mathsf{C}$, and suppose that $$f\circ s=f\circ t.$$Then, $g\circ(f\circ s)=g\circ(f\circ t)$, so by associativity $$(g\circ f)\circ s=(g\circ f)\circ t.$$Since $g\circ f$ is a monomorphism, we have $s=t$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Monomorphism]]