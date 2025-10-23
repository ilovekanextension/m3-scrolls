**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$ and $g:A\to B$. Then, $f=g$ if and only if for all $a\in A$ we have $f(a)=g(a)$.

**Proof of Forward Implication.** Suppose $f=g$. Suppose $a\in A$. By totality of $f$ and $g$, there are objects $b,c\in B$ such that $(a,b)\in f$ and $(a,c)\in g$. Since $f=g$, we have $(a,b)\in f$ and $(a,c)\in f$, so by functionality of $f$ we have $b=c$. Therefore, $f(a)=g(a)$. $\blacksquare$

**Proof of Backward Implication.** Suppose for all $a\in A$ we have $f(a)=g(a)$. Suppose $(a,b)\in A\times B$. We have
$$\begin{align}
(a,b)\in f & \iff b=f(a) \\
 & \iff b=g(a) \\
 & \iff(a,b)\in g.\blacksquare
\end{align}$$
***
Definitions used:
- [[Set]]
- [[Cartesian Product]]
- [[Function]]