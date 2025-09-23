**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $a\in A$.
1. $a$ is the infimum of $B$ under $\leq$ if and only if $a$ is the supremum of $B$ under $\leq^{\text{op}}$.
2. $a$ is the supremum of $B$ under $\leq$ if and only if $a$ is the infimum of $B$ under $\leq^{\text{op}}$.

**Proof of First Statement.** Denote "$a$ is the infimum of $B$ under $\leq$" and "$a$ is the supremum of $B$ under $\leq^\text{op}$" as $(1)$ and $(2)$ respectively. We have
$$\begin{align}
(1) & \iff \forall b\in B \ (a\leq b)\wedge\forall c\in A \ (\forall b\in B \ (c\leq b)\Rightarrow c\leq a) \\
 & \iff \forall b\in B \ (b\leq^\text{op}a)\wedge\forall c\in A \ (\forall b\in B \ (b\leq^\text{op}c)\Rightarrow a\leq c) \\
 & \iff (2).\blacksquare
\end{align}$$

**Proof of Second Statement.** By the first statement, $a$ is the infimum of $B$ under $\leq^{\text{op}}$ if and only if $a$ is the supremum of $B$ under $(\leq^{\text{op}})^\text{op}$. By [[Involution Property on Order Duals]], $(\leq^\text{op})^\text{op}$ is equal to $\leq$. The statement follows immediately. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Inverse of Relation]]
- [[Partial Order]]
- [[Dual Order]]
- [[Infimum]]
- [[Supremum]]

Theorems used:
- [[Involution Property on Order Duals]]