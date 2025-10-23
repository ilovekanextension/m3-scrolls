**Theorem.** Let $A$, $B$, and $C$ be sets. Let $R\subseteq A\times B$ and $S\subseteq B\times C$. Then, $$(S\circ R)^{-1}=R^{-1}\circ S^{-1}.$$
**Proof.** Suppose $(c,a)\in C\times A$. We have
$$\begin{align}
(c,a)\in R^{-1}\circ S^{-1} & \iff \exists b\in B\  (cS^{-1}b\wedge bR^{-1}a) \\
 & \iff \exists b\in B \ (aRb\wedge bSc) \\
 & \iff (a,c)\in S\circ R \\
 & \iff (c,a)\in(S\circ R)^{-1}.\blacksquare
\end{align}$$
***
Definitions used:
- [[Set]]
- [[Cartesian Product]]
- [[Relation]]
- [[Inverse of Relation]]
- [[Composition of Relations]]