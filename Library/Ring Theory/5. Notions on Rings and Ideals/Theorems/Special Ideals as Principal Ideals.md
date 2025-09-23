**Theorem.** Let $R$ be a commutative ring.
1. $\{0\}$ is a principal ideal of $R$. In fact, $\{0\}=(0)$.
2. $R$ is a principal ideal of $R$. In fact, $R=(1)$.

**Proof of First Statement.** By [[Trivial Subgroups]], $\{0\}$ is a subgroup of $R$. Now suppose $r\in R$ and $a\in\{0\}$. This means $a=0$. By [[Multiplications with Ring Zeros]], $r\cdot a=r\cdot 0=0$ and $a\cdot r=0\cdot r=0$, so $r\cdot a\in\{0\}$ and $a\cdot r\in\{0\}$. Therefore, $\{0\}$ is an ideal of $R$.

Observe that
$$\begin{align}
(0) & =\{r\cdot 0\in R\mid r\in R\} \\
 & =\{0\}.
\end{align}$$
This shows that $\{0\}$ is principal. $\blacksquare$

**Proof of Second Statement.** Clearly $R$ is an ideal of $R$. We have
$$\begin{align}
(1) & =\{r\cdot 1\in R\mid r\in R\} \\
 & =R,
\end{align}$$
so $R$ is principal. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Ideal]]
- [[Principal Ideal]]
- [[Subgroup]]
- [[Enumeration Notation]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Trivial Subgroups]]