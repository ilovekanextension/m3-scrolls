**Theorem.** Let $G=(G,\circ)$, $H=(H,+)$, and $I=(I,*)$ be groups. Let $\phi:G\to H$ and $\eta:H\to I$ be group homomorphisms. Then, $\eta\circ \phi$ is also a group homomorphism.

**Proof.** Suppose $a,b\in G$. By [[Evaluations of Composite Functions]],
$$\begin{align}
\eta\circ\phi(a\circ b) & =\eta(\phi(a\circ b)) \\
 & =\eta(\phi(a)+\phi(b)) \\
 & =\eta(\phi(a))*\eta(\phi(b)) \\
 & =\eta\circ\phi(a)*\eta\circ\phi(b).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Composition of Functions]]

Theorems used:
- [[Evaluations of Composite Functions]]