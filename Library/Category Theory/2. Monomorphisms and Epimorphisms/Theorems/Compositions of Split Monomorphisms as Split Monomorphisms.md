**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be split monomorphisms in $\mathsf{C}$. Then, $g\circ f:A\to C$ is also a split monomorphism.

**Proof.** Since $f$ is a split monomorphism, there is $x:B\to A$ such that $x\circ f=\text{id}_{A}$. Since $g$ is a split monomorphism, there is $y:C\to B$ such that $y\circ g=\text{id}_{B}$. Notice that
$$\begin{align}
(x\circ y)\circ(g\circ f) & =x\circ(y\circ(g\circ f)) \\
 & =x\circ((y\circ g)\circ f) \\
 & =x\circ(\text{id}_{B}\circ f) \\
 & =x\circ f \\
 & =\text{id}_{A}. \blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Split Monomorphism]]