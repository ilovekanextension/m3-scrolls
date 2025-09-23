**Theorem.** Let $G$ be a group. Let $A$ be a set. Let $\rho:G\times A\to A$ be a group action of $G$ on $A$. Then, the function $\sigma:G\to S_{A}$ defined as $$\sigma(g)=\rho(g,-)$$is a group homomorphism. Note that $\sigma$ is well-defined by [[Induced Bijective Functions from Group Actions on Sets]].

**Proof.** Suppose $g,h\in G$. By [[Evaluations of Composite Functions]], for all $a\in A$ we have
$$\begin{align}
\sigma(g\circ h)(a) & =\rho(g\circ h,a) \\
 & =\rho(g,\rho(h,a)) \\
 & =\rho(g,\sigma(h)(a)) \\
 & =\sigma(g)(\sigma(h)(a)) \\
 & =\sigma(g)\circ \sigma(h)(a),
\end{align}$$
so by [[Extensionality of Functions]] $\sigma(g\circ h)=\sigma(g)\circ \sigma(h)$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Symmetric Group]]
- [[Group Action on Set]]
- [[Set]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]