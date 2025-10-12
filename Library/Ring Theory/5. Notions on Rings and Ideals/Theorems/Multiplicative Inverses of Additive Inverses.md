**Theorem.** Let $\mathbb{F}$ be a field. Suppose $a\in \mathbb{F}$ is nonzero.
1. $-a$ is nonzero, so $-a$ has a multiplicative inverse.
2. We have $$(-a)^{-1}=-(a^{-1}).$$

**Proof of First Statement.** For the sake of negation, assume that $-a=0$. Then, $-a+a=0+a$, so $0=a$. This contradicts the fact that $a$ is nonzero. Therefore, the assumption that $-a=0$ is false, so $-a$ is nonzero. $\blacksquare$

**Proof of Second Statement.** By [[Multiplications with Additive Inverses]],
$$\begin{align}
(-a)^{-1}\cdot(-a) & =1 \\
 & =a^{-1}\cdot a \\
 & =-(a^{-1})\cdot(-a),
\end{align}$$
so by [[Multiplication Cancellation Properties on Fields]] $(-a)^{-1}=-(a^{-1})$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Field]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Multiplication Cancellation Properties on Fields]]