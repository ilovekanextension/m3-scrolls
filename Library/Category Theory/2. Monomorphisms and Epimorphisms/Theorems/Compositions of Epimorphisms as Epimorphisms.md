**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be epimorphisms in $\mathsf{C}$. Then, $g\circ f:A\to C$ is also an epimorphism.

**Proof.** Suppose $s:C\to X$ and $t:C\to X$ are morphisms in $\mathsf{C}$, and suppose that $$s\circ(g\circ f)\circ s=t\circ(g\circ f).$$Then, by associativity law, we have $$(s\circ g)\circ f=(t\circ g)\circ f.$$Since $f$ is an epimorphism, $s\circ g=t\circ g$. Since $g$ is also an epimorphism, $s=t$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Epimorphism]]

