**Theorem.** Let $G$ be a group. Let $A$ be a set. Let $\rho:G\times A\to A$ be a group action of $G$ on $A$. Then, for all $g\in G$, the function $$\rho(g,-):A\to A$$is bijective.

**Proof.** Suppose $g\in G$. Consider the function $\rho(g^{-1},-):A\to A$. By [[Evaluations of Composite Functions]], for all $a\in A$ we have 
$$\begin{align}
\rho(g^{-1},-)\circ \rho(g,-)(a) & =\rho(g^{-1},\rho(g,a)) \\
 & =\rho(g^{-1}\circ g,a) \\
 & =\rho(1,a) \\
 & =a \\
 & =\text{id}_{A}(a)
\end{align}$$
and 
$$\begin{align}
\rho(g,-)\circ \rho(g^{-1},-)(a) & =\rho(g,\rho(g^{-1},a)) \\
 & =\rho(g\circ g^{-1},a) \\
 & =\rho(1,a) \\
 & =a \\
 & =\text{id}_{A}(a).
\end{align}$$
Therefore, by [[Extensionality of Functions]] and [[Bijective Functions as Isomorphisms]] $\rho(g,-)$ is bijective with inverse $\rho(g^{-1},-)$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Action on Set]]
- [[Set]]
- [[Bijective Function]]
- [[Composition of Functions]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Bijective Functions as Isomorphisms]]