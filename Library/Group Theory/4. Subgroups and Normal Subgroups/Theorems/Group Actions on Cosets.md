**Theorem.** Let $G$ be a group. Let $S$ be a subgroup of $G$.
1. Suppose $X\in G/S$. Then, for all $a\in G$, $a\circ X\in G/S$. In fact, for all $a,b\in G$, $$a\circ(b\circ S)=(a\circ b)\circ S.$$We can therefore construct a function $\sigma:G\times G/S\to G/S$ defined as $\sigma(g,X)=g\circ X$.
2. The function $\sigma$ defined in the first statement is a group action of $G$ on $G/S$.

**Proof of First Statement.** Suppose $a\in G$. Since $X\in G/S$, there is $g\in G$ such that $X=g\circ S$. We will show that $a\circ X=(a\circ g)\circ S$. First suppose $b\in a\circ X$. Then, there is $s\in S$ such that $b=a\circ(g\circ s)$. We then have $$b=(a\circ g)\circ s\in(a\circ g)\circ S.$$Next suppose $b\in(a\circ g)\circ S$. Then, there is $s\in S$ such that $b=(a\circ g)\circ S$. We then have $$b=a\circ(g\circ s)\in a\circ (g\circ S)=a\circ X.\blacksquare$$
**Proof of Second Statement.** First suppose $X\in G/S$. Then, there is $g\in G$ such that $X=g\circ S$. We then have
$$\begin{align}
\sigma(1,X) & =1\circ X \\
 & =1\circ(g\circ S) \\
 & =(1\circ g)\circ S \\
 & =g\circ S \\
 & =X.
\end{align}$$
Next suppose $a,b\in G$ and $X\in G/S$. Then, there is $g\in G$ such that $X=g\circ S$. We then have
$$\begin{align}
\sigma(a\circ b,X) & =(a\circ b)\circ X \\
 & =(a\circ b)\circ(g\circ S) \\
 & =((a\circ b)\circ g)\circ S \\
 & =(a\circ(b\circ g))\circ S \\
 & =a\circ((b\circ g)\circ S) \\
 & =\sigma(a,(b\circ g)\circ S) \\
 & =\sigma(a,b\circ(g\circ S)) \\
 & =\sigma(a,\sigma(b,g\circ S)) \\
 & =\sigma(a,\sigma(b,X)).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Action on Set]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Function]]