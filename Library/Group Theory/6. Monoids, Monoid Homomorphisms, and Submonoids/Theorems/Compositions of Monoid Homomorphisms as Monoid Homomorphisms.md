**Theorem.** Let $M=(M,\circ)$, $N=(N,+)$, and $P=(P,*)$ be monoids. Let $\phi:M\to N$ and $\eta:N\to P$ be monoid homomorphisms. Then, $\eta\circ \phi$ is also a monoid homomorphism.

**Proof.**
- **Preservation of Identities.** By [[Evaluations of Composite Functions]], $$\begin{align}
\eta\circ\phi(1_{M}) & =\eta(\phi(1_{M})) \\
 & =\eta(1_{N}) \\
 & =1_{P}.
\end{align}$$
- **Preservation of Compositions.** Suppose $a,b\in M$. By [[Evaluations of Composite Functions]], $$\begin{align}
\eta\circ\phi(a\circ b) & =\eta(\phi(a\circ b)) \\
 & =\eta(\phi(a)+\phi(b)) \\
 & =\eta(\phi(a))*\eta(\phi(b)) \\
 & =\eta\circ \phi(a)*\eta\circ\phi(b).\blacksquare
\end{align}$$

***
Definitions used:
- [[Monoid]]
- [[Monoid Homomorphism]]
- [[Composition of Functions]]

Theorems used:
- [[Evaluations of Composite Functions]]