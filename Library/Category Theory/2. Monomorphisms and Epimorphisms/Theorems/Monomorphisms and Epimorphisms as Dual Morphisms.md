**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a morphism in $\mathsf{C}$.
1. Suppose that $f$ is a monomorphism in $\mathsf{C}$. Then, $f^\text{op}$ is an epimorphism in $\mathsf{C}^\text{op}$.
2. Suppose that $f$ is an epimorphism in $\mathsf{C}$. Then, $f^\text{op}$ is a monomorphism in $\mathsf{C}^\text{op}$.

Hence, we say that monomorphisms are **dual** to epimorphisms and vice versa.

**Proof of First Statement.** Suppose $s^\text{op}:A\to X$ and $t^\text{op}:A\to X$ are morphisms in $\mathsf{C}^\text{op}$, and suppose that $$s^\text{op}\circ f^\text{op}=t^\text{op}\circ f^\text{op}.$$Then, $(f\circ s)^\text{op}=(f\circ t)^\text{op}$, so $f\circ s=f\circ t$. Since $f$ is a monomorphism, we have $s=t$, so $s^\text{op}=t^\text{op}$. $\blacksquare$

**Proof of Second Statement.** Suppose $s^\text{op}:X\to B$ and $t^\text{op}:X\to B$ are morphisms in $\mathsf{C}^\text{op}$, and suppose that $$f^\text{op}\circ s^\text{op}=f^\text{op}\circ t^\text{op}.$$Then, $(s\circ f)^\text{op}=(t\circ f)^\text{op}$, so $s\circ f=t\circ f$. Since $f$ is an epimorphism, we have $s=t$, so $s^\text{op}=t^\text{op}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Opposite Category]]
- [[Monomorphism]]
- [[Epimorphism]]