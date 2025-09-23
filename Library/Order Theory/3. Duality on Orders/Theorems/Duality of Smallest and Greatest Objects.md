**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $b\in B$.
1. $b$ is the smallest object of $B$ under $\leq$ if and only if $b$ is the greatest object of $B$ under $\leq^{\text{op}}$.
2. $b$ is the greatest object of $B$ under $\leq$ if and only if $b$ is the smallest object of $B$ under $\leq^{\text{op}}$.

**Proof of First Statement.** Denote "$b$ is the smallest object of $B$ under $\leq$" and "$b$ is the greatest object of $\leq^{\text{op}}$" as $(1)$ and $(2)$ respectively. We have
$$\begin{align}
(1) & \iff \forall x\in B \ (b\leq x) \\
 & \iff \forall x\in B \ (x\leq^{\text{op}}b) \\
 & \iff (2).\blacksquare
\end{align}$$

**Proof of Second Statement.** By the first statement, $b$ is the smallest object of $B$ under $\leq^{\text{op}}$ if and only if $b$ is the greatest object of $B$ under $(\leq^\text{op})^\text{op}$. By [[Involution Property on Order Duals]], $(\leq^\text{op})^\text{op}$ is equal to $\leq$. The statement immediately follows. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Inverse of Relation]]
- [[Partial Order]]
- [[Smallest Object]]
- [[Dual Order]]
- [[Greatest Object]]

Theorems used:
- [[Involution Property on Order Duals]]