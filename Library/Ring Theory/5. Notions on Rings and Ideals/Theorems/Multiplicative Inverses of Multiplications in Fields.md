**Theorem.** Let $\mathbb{F}$ be a field. Suppose $a,b\in \mathbb{F}$ are both nonzero.
1. $a\cdot b$ is also nonzero, so $a\cdot b$ has a multiplicative inverse.
2. We have $$(a\cdot b)^{-1}=a^{-1}\cdot b^{-1}.$$

**Proof of First Statement.** For the sake of negation, assume that $a\cdot b=0$. Since $\mathbb{F}$ is a field, by [[Fields as Integral Domains]] $\mathbb{F}$ is an integral domain, so $a=0$ or $b=0$. However, by assumption both $a$ and $b$ are nonzero, so we have a contradiction. This means the assumption that $a\cdot b=0$ must be false, so $a\cdot b$ is nonzero. $\blacksquare$

**Proof of Second Statement.** Since $\mathbb{F}$ is a field, $\mathbb{F}$ is commutative. We therefore have
$$\begin{align}
(a\cdot b)\cdot a^{-1}\cdot b^{-1} & =a\cdot a^{-1}\cdot b\cdot b^{-1} \\
 & =1\cdot 1 \\
 & =1 \\
 & =(a\cdot b)\cdot(a\cdot b)^{-1},
\end{align}$$
so by [[Multiplication Cancellation Properties on Fields]] $a^{-1}\cdot b^{-1}=(a\cdot b)^{-1}$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Integral Domain]]
- [[Field]]

Theorems used:
- [[Multiplication Cancellation Properties on Fields]]
- [[Fields as Integral Domains]]