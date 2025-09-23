**Theorem.** Let $R$ and $S$ be rings. Let $\phi:R\to S$ be a surjective ring homomorphism. Then, as rings, $$\frac{R}{\ker(\phi)}\cong S.$$
**Proof.** By [[First Isomorphism Theorem for Groups]], the function $\eta:R/(\ker(\phi))\to \text{im}(\phi)$ defined as $$\eta(a+\ker(\phi))=\phi(a)$$is a well-defined bijective group homomorphism. We will show that $\eta$ is also a ring homomorphism. From here, we can conclude that $\eta$ is a bijective ring homomorphism, hence a ring isomorphism, so $$\frac{R}{\ker(\phi)}\cong\text{im}(\phi).$$Since $\phi$ is surjective, $\text{im}(\phi)=S$, so the statement follows.

- **Preservation of Multiplications.** Suppose $a,b\in R$. We have $$\begin{align}
\eta((a+\ker(\phi))\cdot(b+\ker(\phi))) & =\eta((a\cdot b)+\ker(\phi)) \\
 & =\phi(a\cdot b) \\
 & =\phi(a)\cdot \phi(b) \\
 & =\eta(a+\ker(\phi))\cdot \eta(b+\ker(\phi))
\end{align}$$
- **Preservation of Multiplicative Identities.** We have $$\begin{align}
\eta(1_{R/(\ker(\phi))}) & =\eta(1_{R}+\ker(\phi)) \\
 & =\phi(1_{R}) \\
 & =1_{S}.\blacksquare
\end{align}$$
***
Definitions used:
- [[Ring]]
- [[Ring Homomorphism]]
- [[Ring Isomorphism]]
- [[Quotient Ring]]
- [[Group Homomorphism]]
- [[Left and Right Coset]]
- [[Surjective Function]]
- [[Image of Function]]

Theorems used:
- [[First Isomorphism Theorem for Groups]]
- [[Kernels of Ring Homomorphisms as Ideals]]