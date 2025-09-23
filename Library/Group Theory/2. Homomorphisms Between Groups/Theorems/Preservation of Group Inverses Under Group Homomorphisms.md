**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$, and suppose that for all $a,b\in G$, $$\phi(a\circ b)=\phi(a)+\phi(b).$$Then, for all $a\in G$, $\phi(a^{-1})=\phi(a)^{-1}$.

**Proof.** Suppose $a\in G$. By [[Preservation of Group Identities Under Group Homomorphisms]],
$$\begin{align}
\phi(a^{-1})+\phi(a) & =\phi(a^{-1}\circ a) \\
 & =\phi(1_{G}) \\
 & =1_{H} \\
 & =\phi(a)^{-1}+\phi(a),
\end{align}$$
so by [[Cancellation Properties on Groups]] $\phi(a^{-1})=\phi(a)^{-1}$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Function]]

Theorems used:
- [[Cancellation Properties on Groups]]
- [[Preservation of Group Identities Under Group Homomorphisms]]