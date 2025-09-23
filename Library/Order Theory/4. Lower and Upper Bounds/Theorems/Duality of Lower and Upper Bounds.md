**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $a\in A$.
1. $a$ is a lower bound for $B$ under $\leq$ if and only if $a$ is an upper bound for $B$ under $\leq^\text{op}$.
2. $a$ is an upper bound for $B$ under $\leq$ if and only if $a$ is a lower bound for $B$ under $\leq^\text{op}$.

**Proof of First Statement.** Denote "$a$ is a lower bound for $B$ under $\leq$" and "$a$ is an upper bound of $B$ under $\leq^\text{op}$" as $(1)$ and $(2)$ respectively. We have
$$\begin{align}
(1) & \iff \forall b\in B \ (a\leq b) \\
 & \iff \forall b\in B \ (b\leq^{\text{op}}a) \\
 & \iff (2).\blacksquare
\end{align}$$

**Proof of Second Statement.** By the first statement, $a$ is a lower bound for $B$ under $\leq^{\text{op}}$ if and only if $a$ is an upper bound for $B$ under $(\leq^\text{op})^{\text{op}}$. By [[Involution Property on Order Duals]], $(\leq^\text{op})^\text{op}$ is equal to $\leq$. The statement immediately follows. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Inverse of Relation]]
- [[Partial Order]]
- [[Dual Order]]
- [[Lower Bound]]
- [[Upper Bound]]

Theorems used:
- [[Involution Property on Order Duals]]