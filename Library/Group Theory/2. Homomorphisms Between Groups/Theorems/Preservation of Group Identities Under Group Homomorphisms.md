**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$, and suppose that for all $a,b\in G$, $$\phi(a\circ b)=\phi(a)+\phi(b).$$Then, $\phi(1_{G})=1_{H}$.

**Proof.** We have
$$\begin{align}
\phi(1_{G})+\phi(1_{G}) & =\phi(1_{G}\circ 1_{G}) \\
 & =\phi(1_{G}) \\
 & =\phi(1_{G})+1_{H},
\end{align}$$
so by [[Cancellation Properties on Groups]] $\phi(1_{G})=1_{H}$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Function]]

Theorems used:
- [[Cancellation Properties on Groups]]