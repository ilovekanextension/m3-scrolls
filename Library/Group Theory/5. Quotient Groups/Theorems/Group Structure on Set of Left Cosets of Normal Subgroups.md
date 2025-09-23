**Theorem.** Let $G$ be a group. Let $N$ be a normal subgroup of $G$.
1. Suppose $a,b,x,y\in G$. Suppose that $a\circ N=x\circ N$ and $b\circ N=y\circ N$. Then, $(a\circ b)\circ N=(x\circ y)\circ N$. We can therefore construct an operation $*:G/N\times G/N\to G/N$ defined as $$(a\circ N)*(b\circ N)=(a\circ b)\circ N.$$
2. Suppose $a,b\in G$, and suppose that $a\circ N=b\circ N$. Then, $a^{-1}\circ N=b^{-1}\circ N$. We can therefore construct a function $(-)^{-1}:G/N\to G/N$ defined as $$(a\circ N)^{-1}=a^{-1}\circ N.$$
3. The set $G/N$ together with the set $N$, the operation $*$ defined on the first statement, and the function $(-)^{-1}$ defined on the second statement forms a group.

**Proof of First Statement.** Since $N$ is normal, we have $N\circ a=N\circ x$, so by [[Criterion for Equality of Cosets]] $a\circ x^{-1}\in N$. By [[Inverses of Group Compositions]], this means $$(a\circ b)\circ(x\circ b)^{-1}=a\circ b\circ b^{-1}\circ x^{-1}=a\circ x^{-1}\in N,$$so by [[Criterion for Equality of Cosets]] again $N\circ(a\circ b)=N\circ(x\circ b)$. Since $N$ is normal, $(a\circ b)\circ N=(x\circ b)\circ N$.

Now observe that, by [[Group Actions on Cosets]],
$$\begin{align}
(x\circ b)\circ N & =x\circ(b\circ N) \\
 & =x\circ(y\circ N) \\
 & =(x\circ y)\circ N.
\end{align}$$
Using transitivity, we can therefore conclude that $(a\circ b)\circ N=(x\circ y)\circ N$. $\blacksquare$

**Proof of Second Statement.** By [[Criterion for Equality of Cosets]], $a^{-1}\circ b\in N$. By [[Involution Property on Group Inverses]] and [[Inverses of Group Compositions]], this means $$b^{-1}\circ(a^{-1})^{-1}=(a^{-1}\circ b)^{-1}\in N.$$Therefore, by [[Criterion for Equality of Cosets]] again $N\circ b^{-1}=N\circ a^{-1}$. Since $N$ is normal, $a^{-1}\circ N=b^{-1}\circ N$. $\blacksquare$

**Proof of Third Statement.**
- **Associativity.** Suppose $X,Y,Z\in G/N$. Then, there are $a,b,c\in G$ such that $X=a\circ N$, $Y=b\circ N$, and $Z=c\circ N$. We then have $$\begin{align}
(X*Y)*Z & =((a\circ N)*(b\circ N))*(c\circ N) \\
 & =((a\circ b)\circ N)*(c\circ N) \\
 & =((a\circ b)\circ c)\circ N \\
 & =(a\circ(b\circ c))\circ N \\
 & =(a\circ N)*((b\circ c)\circ N) \\
 & =(a\circ N)*((b\circ N)*(c\circ N)) \\
 & =X*(Y*Z).
\end{align}$$
- **Existence of Identity.** Suppose $X\in G/N$. Then, there is $a\in G$ such that $X=a\circ N$. By [[Group Actions on Cosets]], $N=1\circ N$, so $$N*X=(1\circ N)*(a\circ N)=(1\circ a)\circ N=a\circ N=X$$and $$X*N=(a\circ N)*(1\circ N)=(a\circ 1)\circ N=a\circ N=X.\blacksquare$$
- **Existence of Inverses.** Suppose $X\in G/N$. Then, there is $a\in G$ such that $X=a\circ N$. By [[Group Actions on Cosets]], $N=1\circ N$, so $$X^{-1}*X=(a\circ N)^{-1}*(a\circ N)=(a^{-1}\circ N)*(a\circ N)=(a^{-1}\circ a)\circ N=1\circ N=N$$and $$X*X^{-1}=(a\circ N)*(a\circ N)^{-1}=(a\circ N)*(a^{-1}\circ N)=(a\circ a^{-1})\circ N=1\circ N=N.\blacksquare$$

***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Normal Subgroup]]
- [[Function]]

Theorems used:
- [[Involution Property on Group Inverses]]
- [[Inverses of Group Compositions]]
- [[Criterion for Equality of Cosets]]
- [[Group Actions on Cosets]]