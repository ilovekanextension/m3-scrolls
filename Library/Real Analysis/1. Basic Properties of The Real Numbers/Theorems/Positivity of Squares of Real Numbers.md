**Theorem.**
1. Suppose $a\in \mathbb{R}$. Then, $a\cdot a\geq 0$.
2. $1>0$.

**Proof of First Statement.** By [[Closure and Trichotomy Properties of Positive Real Numbers]], we have $a\in \mathbb{R}^+$ or $-a\in \mathbb{R}^+$ or $a=0$. We proceed by cases; in each case we will show that $a\cdot a\geq 0$.
- **Case** $a\in \mathbb{R}^+$. This means $a>0$. By the second order property, we then have $a\cdot a>a\cdot 0$, so by [[Multiplications with Ring Zeros]] $a\cdot a>0$. Therefore, $a\cdot a>0$ or $a\cdot a=0$, so $a\cdot a\geq 0$.
- **Case** $-a\in \mathbb{R}^+$. This means $-a>0$. By the second order property, we then have $(-a)\cdot(-a)>0$, so by [[Multiplications with Ring Zeros]] and [[Multiplications with Additive Inverses]] $a\cdot a>0$. Therefore, $a\cdot a>0$ or $a\cdot a=0$, so $a\cdot a\geq 0$.
- **Case** $a=0$. By [[Multiplications with Ring Zeros]], this means $a\cdot a=0$. Therefore, $a\cdot a>0$ or $a\cdot a=0$, so $a\cdot a\geq 0$. $\blacksquare$

**Proof of Second Statement.** Since $1=1\cdot 1$, by the first statement $1\geq 0$, so $1>0$ or $1=0$. Since $\mathbb{R}$ is a field, by definition it is nontrivial, so $1\neq 0$. Therefore, we must have $1> 0$. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Field]]

Theorems used:
- [[Closure and Trichotomy Properties of Positive Real Numbers]]
- [[Multiplications with Ring Zeros]]
- [[Multiplications with Additive Inverses]]