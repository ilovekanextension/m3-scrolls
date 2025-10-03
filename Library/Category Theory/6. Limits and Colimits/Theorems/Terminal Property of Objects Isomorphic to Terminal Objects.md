**Theorem.** Let $\mathsf{C}$ be a category. Let $a$ and $t$ be objects in $\mathsf{C}$. Suppose that $t$ is terminal, and suppose that $a\cong t$. Then, $a$ is terminal.

**Proof.** Suppose $b$ is an object in $\mathsf{C}$.
- **Existence.** Since $t$ is terminal, there is a morphism $f:b\to t$. Since $a\cong t$, there is an isomorphism $g:a\to t$, so there is a morphism $g^{-1}\circ f:b\to a$.
- **Uniqueness.** Suppose $h:b\to a$ and $k:b\to a$ are morphisms in $\mathsf{C}$. We then have morphisms $g\circ h:b\to t$ and $g\circ k:b\to t$. Since $t$ is terminal, we must have $g\circ h=g\circ k$. By [[Isomorphisms as Two Sided Invertible Morphisms]] and [[Split Monomorphisms as Monomorphisms]], $g$ is a monomorphism, so $h=k$. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Terminal Object]]