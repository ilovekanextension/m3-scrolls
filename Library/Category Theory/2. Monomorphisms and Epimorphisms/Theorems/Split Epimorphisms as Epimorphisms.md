**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a split epimorphism in $\mathsf{C}$. Then, $f$ is also an epimorphism.

**Proof.** Suppose $s:B\to X$ and $t:B\to X$ are morphisms in $\mathsf{C}$, and suppose that $s\circ f=t\circ f$. Since $f$ is a split epimorphism, there is $g:B\to A$ such that $f\circ g=\text{id}_{B}$. Since $s\circ f=t\circ f$, we have
$$\begin{align}
&& (s\circ f)\circ g & =(t\circ f)\circ g \\
\Rightarrow && s\circ(f\circ g) & =t\circ(f\circ g) \\
\Rightarrow && s\circ \text{id}_{B} & =t\circ \text{id}_{B} \\
\Rightarrow && s & =t.\blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Epimorphism]]
- [[Split Epimorphism]]