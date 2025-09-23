**Theorem.** Let $A$, $B$, and $C$ be sets. Then, $$(A\cup B)\cup C=A\cup(B\cup C).$$
**Proof.** Suppose $x$ is an object. We have
$$\begin{align}
x\in(A\cup B)\cup C & \iff x\in A\cup B\vee x\in C \\
 & \iff (x\in A\vee x\in B)\vee x\in C \\
 & \iff x\in A\vee(x\in B\vee x\in C) \\
 & \iff x\in A\vee x\in B\cup C \\
 & \iff x\in A\cup(B\cup C). \blacksquare
\end{align}$$
***
Definitions used:
- [[Set]]
- [[Union of Two Sets]]