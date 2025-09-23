**Theorem.** Let $G$ be a group. Let $A$ be a set. Let $\phi:G\to S_{A}$ be a group homomorphism. Then, the function $\rho:G\times A\to A$ defined as $$\rho(g,a)=\phi(g)(a)$$is a group action of $G$ on $A$.

**Proof.** First suppose $a\in A$. We have
$$\begin{align}
\rho(1_{G},a) & =\phi(1_{G})(a) \\
 & =1_{S_{A}}(a) \\
 & =\text{id}_{A}(a) \\
 & =a.
\end{align}$$
Next suppose $g,h\in G$ and $a\in A$. By [[Evaluations of Composite Functions]],
$$\begin{align}
\rho(g\circ h,a) & =\phi(g\circ h)(a) \\
 & =(\phi(g)\circ \phi(h))(a) \\
 & =\phi(g)(\phi(h)(a)) \\
 & =\rho(g,\phi(h,a)) \\
 & =\rho(g,\rho(h,a)).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Group Action on Set]]
- [[Set]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Evaluations of Composite Functions]]