**Theorem.** Let $R$ be a ring.
1. For all $a,b\in R$, $-a\cdot b=-(a\cdot b)$ and $a\cdot(-b)=-(a\cdot b)$.
2. For all $a,b\in R$, $-a\cdot(-b)=a\cdot b$.

**Proof of First Statement.** Suppose $a,b\in R$. By [[Multiplications with Ring Zeros]],
$$\begin{align}
-a\cdot b+a\cdot b & =(-a+a)\cdot b \\
 & =0\cdot b \\
 & =0 \\
 & =-(a\cdot b)+a\cdot b,
\end{align}$$
so by [[Cancellation Properties on Groups]] $-a\cdot b=-(a\cdot b)$. Likewise, by [[Multiplications with Ring Zeros]],
$$\begin{align}
a\cdot(-b)+a\cdot b & =a\cdot(-b+b) \\
 & =a\cdot 0 \\
 & =0 \\
 & =-(a\cdot b)+a\cdot b,
\end{align}$$
so by [[Cancellation Properties on Groups]] $a\cdot(-b)=-(a\cdot b)$. $\blacksquare$

**Proof of Second Statement.** Suppose $a,b\in R$. By the first statement and [[Multiplications with Ring Zeros]],
$$\begin{align}
-a\cdot(-b)+ (-a)\cdot b & =-a\cdot(-b+b) \\
 & =-a\cdot 0 \\
 & =0 \\
 & =a\cdot b+(-(a\cdot b)) \\
 & =a\cdot b+(-a)\cdot b,
\end{align}$$
so by [[Cancellation Properties on Groups]] $-a\cdot(-b)=a\cdot b$. $\blacksquare$
***
Definitions used:
- [[Ring]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Cancellation Properties on Groups]]