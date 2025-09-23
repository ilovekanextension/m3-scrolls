**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ and $g:b\to c$ be monomorphisms in $\mathsf{C}$. Then, $g\circ f:a\to c$ is also a monomorphism.

**Proof.** Suppose $s:x\to a$ and $t:x\to a$ are morphisms in $\mathsf{C}$, and suppose that $$(g\circ f)\circ s=(g\circ f)\circ t.$$Then, by associativity law, we have $$g\circ(f\circ s)=g\circ (f\circ t).$$Since $g$ is a monomorphism, $f\circ s=f\circ t$. Since $f$ is also a monomorphism, $s=t$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Monomorphism]]

