**Theorem.** Let $G$ be a group. Then, the composition $\circ:G\times G\to G$ is a group action of $G$ on $G$.

**Proof.** First suppose $a\in G$. We have $$\circ(1,a)=1\circ a=a.$$Next suppose $g,h\in G$ and $a\in G$. We have
$$\begin{align}
\circ(g\circ h,a) & =(g\circ h)\circ a \\
 & =g\circ(h\circ a) \\
 & =\circ(g,h\circ a) \\
 & =\circ(g,\circ(h,a)).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Action on Set]]