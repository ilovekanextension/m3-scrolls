**Theorem.** Let $G$ be a group. Suppose $a,b,c\in G$.
1. Suppose $a\circ b=a\circ c$. Then, $b=c$.
2. Suppose $b\circ a=c\circ a$. Then, $b=c$.

**Proof of First Statement.** We have
$$\begin{align}
b & =1\circ b \\
 & =(a^{-1}\circ a)\circ b \\
 & =a^{-1}\circ (a\circ b) \\
 & =a^{-1}\circ(a\circ c) \\
 & =(a^{-1}\circ a)\circ c \\
 & =1\circ c \\
 & =c.\blacksquare
\end{align}$$

**Proof of Second Statement.** We have
$$\begin{align}
b & =b\circ 1 \\
 & =b\circ(a\circ a^{-1}) \\
 & =(b\circ a)\circ a^{-1} \\
 & =(c\circ a)\circ a^{-1} \\
 & =c\circ(a\circ a^{-1}) \\
 & =c\circ 1 \\
 & =c.\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]