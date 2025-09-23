**Theorem.** Let $R$ and $S$ be rings. Let $\phi:R\to S$ be a ring homomorphism. Then, $\ker(\phi)$ is an ideal of $R$.

**Proof.** By [[Kernels of Group Homomorphisms as Subgroups]], $\ker(\phi)$ is a subgroup of $(R,+)$. Now suppose $r\in R$ and $a\in \ker(\phi)$. Since $a\in\ker(\phi)$, we have $\phi(a)=0_{S}$. By [[Multiplications with Ring Zeros]],
$$\begin{align}
\phi(r\cdot a) & =\phi(r)\cdot \phi(a) \\
 & =\phi(r)\cdot 0_{S} \\
 & =0_{S}
\end{align}$$
and
$$\begin{align}
\phi(a\cdot r) & =\phi(a)\cdot \phi(r) \\
 & =\phi(a)\cdot 0_{S} \\
 & =0_{S},
\end{align}$$
so $r\cdot a\in\ker(\phi)$ and $a\cdot r\in\ker(\phi)$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Ring Homomorphism]]
- [[Ideal]]
- [[Kernel of Group Homomorphism]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Kernels of Group Homomorphisms as Subgroups]]