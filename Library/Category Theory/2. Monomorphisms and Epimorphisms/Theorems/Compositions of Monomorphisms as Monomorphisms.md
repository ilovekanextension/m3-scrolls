**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be monomorphisms in $\mathsf{C}$. Then, $g\circ f:A\to C$ is also a monomorphism.

**Proof.** Suppose $s:X\to A$ and $t:X\to A$ are morphisms in $\mathsf{C}$, and suppose that $$(g\circ f)\circ s=(g\circ f)\circ t.$$Then, by associativity law, we have $$g\circ(f\circ s)=g\circ (f\circ t).$$Since $g$ is a monomorphism, $f\circ s=f\circ t$. Since $f$ is also a monomorphism, $s=t$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Monomorphism]]

