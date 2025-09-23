**Theorem.** Let $\mathbb{F}$ be a field. Then, $\mathbb{F}$ is also an integral domain.

**Proof.** Suppose $a,b\in \mathbb{F}$, and suppose that $a\cdot b=0$. Either $a=0$ or $a\neq 0$. We proceed by cases; in each case we will show that $a=0$ or $b=0$.
- **Case** $a=0$. This means $a=0$ or $b=0$.
- **Case** $a\neq 0$. Since $\mathbb{F}$ is a field, by [[Multiplications with Ring Zeros]] $$b=1\cdot b=a^{-1}\cdot a\cdot b=a^{-1}\cdot 0=0,$$so $a=0$ or $b=0$. $\blacksquare$

***
Definitions used:
- [[Ring]]
- [[Integral Domain]]
- [[Field]]

Theorems used:
- [[Multiplications with Ring Zeros]]