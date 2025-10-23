**Theorem.** Let $A$, $B$, $C$, and $D$ be sets. Let $R\subseteq A\times B$, $S\subseteq B\times C$, and $T\subseteq C\times D$. Then, $$(T\circ S)\circ R=T\circ(S\circ R).$$
**Proof.** Suppose $(a,d)\in A\times D$. We have
$$\begin{align}
(a,d)\in(T\circ S)\circ R & \iff \exists b\in B \ (aRb\wedge b(T\circ S)d) \\
 & \iff \exists b\in B \ \exists c\in C \ (aRb\wedge(bSc\wedge cTd)) \\
 & \iff \exists b\in B \ \exists c\in C \ ((aRb\wedge bSc)\wedge cTd) \\
 & \iff \exists c\in C \ (a(S\circ R)c\wedge cTd) \\
 & \iff (a,d)\in T\circ(S\circ R).\blacksquare
\end{align}$$
***
Definitions used:
- [[Set]]
- [[Cartesian Product]]
- [[Relation]]
- [[Composition of Relations]]