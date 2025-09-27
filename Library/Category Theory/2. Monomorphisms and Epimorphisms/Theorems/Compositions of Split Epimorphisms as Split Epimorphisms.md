**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ and $g:B\to C$ be split epimorphisms in $\mathsf{C}$. Then, $g\circ f:A\to C$ is also a split epimorphism.

**Proof.** Since $f$ is a split epimorphism, there is $x:B\to A$ such that $f\circ x=\text{id}_{B}$. Since $g$ is a split epimorphism, there is $y:C\to B$ such that $g\circ y=\text{id}_{C}$. Notice that
$$\begin{align}
(g\circ f)\circ(x\circ y) & =g\circ(f\circ(x\circ y)) \\
 & =g\circ((f\circ x)\circ y) \\
 & =g\circ(\text{id}_{B}\circ y) \\
 & =g\circ y \\
 & =\text{id}_{C}. \blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Split Epimorphism]]