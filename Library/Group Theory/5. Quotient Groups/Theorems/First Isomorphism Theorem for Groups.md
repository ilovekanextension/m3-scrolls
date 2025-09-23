**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism.
1. Suppose $a,b\in G$, and suppose that $a\circ\ker(\phi)=b\circ\ker(\phi)$. Then, $\phi(a)=\phi(b)$. We can therefore construct a function $\eta:G/\ker(\phi)\to \text{im}(\phi)$ defined as $$\eta(a\circ\ker(\phi))=\phi(a).$$
2. The function $\eta$ defined in the first statement is a group isomorphism.
3. Suppose that $\phi$ is surjective. Then, as groups, $$\frac{G}{\ker(\phi)}\cong H.$$

**Proof of First Statement.** By [[Criterion for Equality of Cosets]], $a^{-1}\circ b\in\ker(\phi)$, so $\phi(a^{-1}\circ b)=1_{H}$. This means $$\phi(a)^{-1}\circ \phi(b)=1_{H},$$so $\phi(a)=\phi(b)$. $\blacksquare$

**Proof of Second Statement.** We first show that $\eta$ is a group homomorphism. Suppose $a,b\in G$. We have
$$\begin{align}
\eta((a\circ\ker(\phi))*(b\circ\ker(\phi))) & =\eta((a\circ b)\circ\ker(\phi)) \\
 & =\phi(a\circ b) \\
 & =\phi(a)+\phi(b) \\
 & =\eta(a\circ\ker(\phi))+\eta(b\circ\ker(\phi)).
\end{align}$$
We first show that $\eta$ is bijective.
- **Injectivity.** Suppose $a,b\in G$, and suppose that $\eta(a\circ\ker(\phi))=\eta(b\circ\ker(\phi))$. Then, $\phi(a)=\phi(b)$. This means $$\phi(a^{-1}\circ b)=\phi(a)^{-1}+\phi(b)=1_{H},$$so $a^{-1}\circ b\in\ker(\phi)$. Therefore, by [[Criterion for Equality of Cosets]] $a\circ\ker(\phi)=b\circ\ker(\phi)$.
- **Surjectivity.** Suppose $b\in \text{im}(\phi)$. Then, there is $a\in G$ such that $b=\phi(a)$. This means $\eta(a\circ\ker(\phi))=\phi(a)=b$. $\blacksquare$

**Proof of Third Statement.** Since $\phi$ is surjective, $\text{im}(\phi)=H$. By the second statement, $$G/\ker(\phi)\cong \text{im}(\phi),$$so $G/\ker(\phi)\cong H$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Group Isomorphism]]
- [[Left and Right Coset]]
- [[Kernel of Group Homomorphism]]
- [[Quotient Group]]
- [[Bijective Function]]

Theorems used:
- [[Criterion for Equality of Cosets]]
- [[Kernels of Group Homomorphisms as Normal Subgroups]]