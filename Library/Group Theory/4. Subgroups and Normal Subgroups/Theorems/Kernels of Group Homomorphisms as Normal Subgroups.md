**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism. Then, $\ker(\phi)$ is a normal subgroup of $G$.

**Proof.** Suppose $a\in G$ and $n\in\ker(\phi)$. Since $n\in\ker(\phi)$, $\phi(n)=1_{H}$. This means
$$\begin{align}
\phi(a\circ n\circ a^{-1}) & =\phi(a)+\phi(n)+\phi(a^{-1}) \\
 & =\phi(a)+1_{H}+\phi(a)^{-1} \\
 & =1_{H}.
\end{align}$$
Therefore, $a\circ n\circ a^{-1}\in\ker(\phi)$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Kernel of Group Homomorphism]]
- [[Normal Subgroup]]