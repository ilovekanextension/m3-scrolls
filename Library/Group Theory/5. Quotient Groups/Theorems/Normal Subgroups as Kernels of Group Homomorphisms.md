**Theorem.** Let $G=(G,\circ)$ be a group. Let $N$ be a subgroup of $G$. Then, $N$ is normal if and only if there is a group $H=(H,+)$ and a group homomorphism $\phi:G\to H$ such that $\ker(\phi)=N$.

**Proof of Forward Implication.** Suppose $N$ is normal. Then, by [[Projection Functions on Quotient Groups as Group Homomorphisms]], the function $\phi:G\to G/N$ defined as $$\phi(a)=a\circ N$$is a group homomorphism. We will show that $\ker(\phi)=N$. By [[Criterion for Equality of Cosets]] and [[Inverses of Group Identities]],
$$\begin{align}
\ker(\phi) & =\{a\in G\mid \phi(a)=1_{G/N}\} \\
 & =\{a\in G\mid a\circ N=N\} \\
 & =\{a\in G\mid a\circ N=1\circ N\} \\
 & =\{a\in G\mid 1^{-1}\circ a\in N\} \\
 & =\{a\in G\mid a\in N\} \\
 & =N.\blacksquare
\end{align}$$

**Proof of Backward Implication.** Suppose there is a group $H=(H,+)$ and a group homomorphism $\phi:G\to H$ such that $\ker(\phi)=N$. Suppose $a\in G$ and $n\in N$. Then, $n\in\ker(\phi)$, so $\phi(n)=1_{H}$. This means
$$\begin{align}
\phi(a\circ n\circ a^{-1}) & =\phi(a)+\phi(n)+\phi(a^{-1}) \\
 & =\phi(a)+1_{H}+\phi(a)^{-1} \\
 & =1_{H}.
\end{align}$$
This means $a\circ n\circ a^{-1}\in \ker(\phi)=N$. Therefore, $N$ is normal. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Kernel of Group Homomorphism]]
- [[Normal Subgroup]]
- [[Quotient Group]]

Theorems used:
- [[Inverses of Group Identities]]
- [[Criterion for Equality of Cosets]]
- [[Projection Functions on Quotient Groups as Group Homomorphisms]]