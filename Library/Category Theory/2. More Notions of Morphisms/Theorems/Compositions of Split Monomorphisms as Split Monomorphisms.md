**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ and $g:b\to c$ be split monomorphisms in $\mathsf{C}$. Then, $g\circ f:a\to c$ is also a split monomorphism.

**Proof.** Since $f$ is a split monomorphism, there is $x:b\to a$ such that $x\circ f=\text{id}_{a}$. Since $g$ is a split monomorphism, there is $y:c\to b$ such that $y\circ g=\text{id}_{b}$. Notice that
$$\begin{align}
(x\circ y)\circ(g\circ f) & =x\circ(y\circ(g\circ f)) \\
 & =x\circ((y\circ g)\circ f) \\
 & =x\circ(\text{id}_{b}\circ f) \\
 & =x\circ f \\
 & =\text{id}_{a}. \blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Split Monomorphism]]