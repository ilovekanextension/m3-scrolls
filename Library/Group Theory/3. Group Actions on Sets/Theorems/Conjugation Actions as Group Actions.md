**Theorem.** Let $G$ be a group. Then, the function $\rho:G\times G\to G$ defined as $$\rho(g,a)=g\circ a\circ g^{-1}$$is a group action of $G$ on $G$.

**Proof.** First suppose $a\in G$. By [[Inverses of Group Identities]], $$\rho(1,a)=1\circ a\circ 1^{-1}=a.$$Next suppose $g,h\in G$ and $a\in G$. By [[Inverses of Group Compositions]],
$$\begin{align}
\rho(g\circ h,a) & =(g\circ h)\circ a\circ(g\circ h)^{-1} \\
 & =g\circ h\circ a\circ h^{-1}\circ g \\
 & =g\circ \rho(h,a)\circ g^{-1} \\
 & =\rho(g,\rho(h,a)).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Action on Set]]

Theorems used:
- [[Inverses of Group Identities]]
- [[Inverses of Group Compositions]]