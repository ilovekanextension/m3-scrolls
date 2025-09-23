**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$ be bijective. Suppose $T\subseteq B$. Then, $$\{f^{-1}(x)\in A\mid x\in T\}=\{x\in A\mid f(x)\in T\}.$$
**Proof.** Suppose $a\in A$. By [[Values of Inverse Functions]] we have
$$\begin{align}
a\in \{f^{-1}(x)\in A\mid x\in T\} & \iff \exists x\in T \ (a=f^{-1}(x)) \\
 & \iff \exists x\in T \ (x=f(a)) \\
 & \iff f(a)\in T \\
 & \iff a\in\{x\in A\mid f(x)\in T\}. \blacksquare
\end{align}$$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Function]]
- [[Bijective Function]]
- [[Inverse of Bijective Function]]

Theorems used:
- [[Values of Inverse Functions]]