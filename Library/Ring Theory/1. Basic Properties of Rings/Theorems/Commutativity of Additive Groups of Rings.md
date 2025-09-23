**Theorem.** Let $R$ be a set. Let $0,1\in R$. Let $+:R\times R\to R$ and $\cdot:R\times R\to R$. Let $-(-):R\to R$. Suppose that
- $(R,+,0,-(-))$ is a group,
- $(R,\cdot,1)$ is a monoid,
- for all $a,b,c\in R$, $$a\cdot(b+c)=a\cdot b+a\cdot c,$$and
- for all $a,b,c\in R$, $$(a+b)\cdot c=a\cdot c+b\cdot c.$$

Then, $(R,+,0,-(-))$ is abelian. That is, for all $a,b\in R$, $a+b=b+a$.

**Proof.** Consider the expression $$(1+1)\cdot(a+b).$$We have
$$\begin{align}
(1+1)\cdot(a+b) & =(1+1)\cdot a+(1+1)\cdot b \\
 & =1\cdot a+1\cdot a+1\cdot b+1\cdot b \\
 & =a+a+b+b
\end{align}$$
and
$$\begin{align}
(1+1)\cdot(a+b) & =1\cdot(a+b)+1\cdot(a+b) \\
 & =1\cdot a+1\cdot b+1\cdot a+1\cdot b \\
 & =a+b+a+b.
\end{align}$$
Therefore, $$a+a+b+b=a+b+a+b,$$so by [[Cancellation Properties on Groups]] $a+b=b+a$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Group]]
- [[Abelian Group]]
- [[Monoid]]

Theorems used:
- [[Cancellation Properties on Groups]]