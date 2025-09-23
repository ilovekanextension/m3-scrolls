**Theorem.** Let $R$ be a ring. Let $I$ be an ideal of $R$. Then, $R/I$ is trivial if and only if $I=(1)$.

**Proof of Forward Implication.** Suppose $R/I$ is trivial.

By [[Special Ideals as Principal Ideals]], $(1)=R$, so $I\subseteq(1)$. Now suppose $x\in(1)$. Then, $x+I\in R/I$. Since $R/I$ is trivial, $0+I=1+I$, so by [[Triviality of Rings with Identical Zeros and Ones]] $R/I=\{0+I\}$. We have $x+I\in R/I$, so $x+I=0+I$. By [[Criterion for Equality of Cosets]] this means $x\in I$. $\blacksquare$

**Proof of Backward Implication.** Suppose $I=(1)$. By [[Special Ideals as Principal Ideals]], $(1)=R$, so $I=R$. Thus, $R/I=R/R$. Notice that
$$\begin{align}
0+R & =\{0+r\in R\mid r\in R\} \\
 & =\{r\in R\mid r\in R\} \\
 & =R \\
 & =\{1+r\in R\mid r\in R\} \\
 & =1+R,
\end{align}$$
so $R/R=R/I$ is trivial. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Trivial Ring]]
- [[Ideal]]
- [[Quotient Ring]]
- [[Left and Right Coset]]
- [[Enumeration Notation]]

Theorems used:
- [[Triviality of Rings with Identical Zeros and Ones]]
- [[Special Ideals as Principal Ideals]]
- [[Criterion for Equality of Cosets]]