**Theorem.** Let $\mathbb{F}$ be a field. Suppose $a\in \mathbb{F}$ is nonzero.
1. $a^{-1}$ is also nonzero, so $a^{-1}$ has a multiplicative inverse.
2. We have $$(a^{-1})^{-1}=a.$$

**Proof of First Statement.** For the sake of negation, assume that $a^{-1}=0$. Then, by [[Multiplications with Ring Zeros]],
$$\begin{align}
a & =a\cdot 1 \\
 & =a\cdot a\cdot a^{-1} \\
 & =a\cdot a\cdot 0 \\
 & =a\cdot 0 \\
 & =0,
\end{align}$$
which contradicts the fact that $a$ is nonzero. Therefore, the assumption that $a^{-1}=0$ must be false, so $a^{-1}$ is nonzero. $\blacksquare$

**Proof of Second Statement.** We have $$(a^{-1})^{-1}\cdot a^{-1}=1=a\cdot a^{-1},$$so by [[Multiplication Cancellation Properties on Fields]] $(a^{-1})^{-1}=a$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Field]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Multiplication Cancellation Properties on Fields]]