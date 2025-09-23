**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ and $g:b\to c$ be isomorphisms in $\mathsf{C}$. Then, $g\circ f:a\to c$ is also an isomorphism and $$(g\circ f)^{-1}=f^{-1}\circ g^{-1}.$$
**Proof.** We have
$$\begin{align}
(g\circ f)\circ(f^{-1}\circ g^{-1}) & =((g\circ f)\circ f^{-1})\circ g^{-1} \\
 & =(g\circ(f\circ f^{-1}))\circ g^{-1} \\
 & =(g\circ \text{id}_{b})\circ g^{-1} \\
 & =g\circ g^{-1} \\
 & =\text{id}_{c}
\end{align}$$
and
$$\begin{align}
(f^{-1}\circ g^{-1})\circ(g\circ f) & =f^{-1}\circ(g^{-1}\circ(g\circ f)) \\
 & =f^{-1}\circ((g^{-1}\circ g)\circ f) \\
 & =f^{-1}\circ(\text{id}_{b}\circ f) \\
 & =f^{-1}\circ f \\
 & =\text{id}_{a}.
\end{align}$$
Therefore, $g\circ f$ is an isomorphism with inverse $f^{-1}\circ g^{-1}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]