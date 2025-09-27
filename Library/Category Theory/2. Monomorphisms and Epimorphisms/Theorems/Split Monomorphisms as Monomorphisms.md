**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a split monomorphism in $\mathsf{C}$. Then, $f$ is also a monomorphism.

**Proof.** Suppose $s:X\to A$ and $t:X\to A$ are morphisms in $\mathsf{C}$, and suppose that $f\circ s=f\circ t$. Since $f$ is a split monomorphism, there is $g:B\to A$ such that $g\circ f=\text{id}_{A}$. Since $f\circ s=f\circ t$, we have
$$\begin{align}
&& g\circ(f\circ s) & =g\circ(f\circ t) \\
\Rightarrow && (g\circ f)\circ s & =(g\circ f)\circ t \\
\Rightarrow && \text{id}_{A}\circ s & =\text{id}_{A}\circ t \\
\Rightarrow && s & =t.\blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Monomorphism]]
- [[Split Monomorphism]]