**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ be a split monomorphism in $\mathsf{C}$. Then, $f$ is also a monomorphism.

**Proof.** Suppose $s:x\to a$ and $t:x\to a$ are morphisms in $\mathsf{C}$, and suppose that $f\circ s=f\circ t$. Since $f$ is a split monomorphism, there is $g:b\to a$ such that $g\circ f=\text{id}_{a}$. Since $f\circ s=f\circ t$, we have
$$\begin{align}
s & =\text{id}_{a}\circ s \\
 & =(g\circ f)\circ s \\
 & =g\circ(f\circ s) \\
 & =g\circ(f\circ t) \\
 & =(g\circ f)\circ t \\
 & =\text{id}_{a}\circ t \\
 & =t. \blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Monomorphism]]
- [[Split Monomorphism]]