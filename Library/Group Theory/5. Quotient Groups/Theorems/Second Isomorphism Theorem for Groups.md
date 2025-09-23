**Theorem.** Let $G$ be a group. Let $S$ and $N$ be subgroups of $G$, and suppose that $N$ is normal. Then, as groups, $$\frac{S}{S\cap N}\cong \frac{S\circ N}{N}.$$
**Proof.** By [[Products With Normal Subgroups as Subgroups]], the quotient groups posed in the statement are well-defined. Consider the function $\phi:S\to(S\circ N)/N$ defined as $$\phi(a)=a\circ N.$$We will first show that $\phi$ is a group homomorphism. Suppose $a,b\in S$. We have
$$\begin{align}
\phi(a\circ b) & =(a\circ b)\circ N \\
 & =(a\circ N)*(b\circ N) \\
 & =\phi(a)*\phi(b).
\end{align}$$
Next, we show that $\phi$ is surjective. Suppose $X\in(S\circ N)/N$. Then, there is $a\in S\circ N$ such that $X=a\circ N$. Since $a\in S\circ N$, there are $s\in S$ and $n\in N$ such that $a=s\circ n$. We will show that $X=s\circ N$; from this, we then have $\phi(s)=X$.

First suppose $x\in X$. Then, there is $m\in N$ such that $x=a\circ m$. We then have $$x=s\circ n\circ m\in s\circ N.$$Next suppose $x\in s\circ N$. Then, there is $m\in N$ such that $x=s\circ m$. Since $a=s\circ n$, we have $s=a\circ n^{-1}$, so $$x=a\circ n^{-1}\circ m\in a\circ N.$$
Since $\phi$ is a surjective group homomorphism, by [[First Isomorphism Theorem for Groups]] $$\frac{S}{\ker(\phi)}\cong\frac{S\circ N}{N}.$$Observe that, by [[Inverses of Group Identities]], [[Criterion for Equality of Cosets]], and [[Group Actions on Cosets]],
$$\begin{align}
\ker(\phi) & =\{a\in S\mid \phi(a)=1_{(S\circ N)/N}\} \\
 & =\{a\in S\mid a\circ N=N\} \\
 & =\{a\in S\mid a\circ N=1\circ N\} \\
 & =\{a\in S\mid 1^{-1}\circ a\in N\} \\
 & =\{a\in S\mid a\in N\} \\
 & =S\cap N.\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Group Isomorphism]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Kernel of Group Homomorphism]]
- [[Normal Subgroup]]
- [[Quotient Group]]

Theorems used:
- [[Inverses of Group Identities]]
- [[Criterion for Equality of Cosets]]
- [[Group Actions on Cosets]]
- [[First Isomorphism Theorem for Groups]]
- [[Products With Normal Subgroups as Subgroups]]