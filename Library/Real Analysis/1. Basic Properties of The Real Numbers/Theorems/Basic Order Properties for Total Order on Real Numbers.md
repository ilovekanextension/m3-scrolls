**Theorem.** Let $a,b,c\in \mathbb{R}$.
1. Suppose $a\leq b$. Then, $a+c\leq b+c$.
2. Suppose $a\leq b$ and $0\leq c$. Then, $a\cdot c\leq b\cdot c$.

**Proof of First Statement.** Since $a\leq b$, by definition $a<b$ or $a=b$. We proceed by cases; in each case we will show that $a+c\leq b+c$.
- **Case** $a<b$. By the first order property, this means $a+c<b+c$, so $a+c\leq b+c$.
- **Case** $a=b$. This means $a+c=b+c$, so $a+c\leq b+c$. $\blacksquare$

**Proof of Second Statement.** Since $a\leq b$, by definition $a<b$ or $a=b$. Likewise, since $0\leq c$, we have $0<c$ or $0=c$. We proceed by cases on the first disjunction; in each case we will show that $a\cdot c\leq b\cdot c$.
- **Case** $a<b$. If $0<c$, then by the second order property $a\cdot c<b\cdot c$, so $a\cdot c\leq b\cdot c$. If $0=c$, then by [[Multiplications with Ring Zeros]] $$a\cdot c=a\cdot 0=0=b\cdot 0=b\cdot c,$$so $a\cdot c\leq b\cdot c$.
- **Case** $a=b$. This means $a\cdot c=b\cdot c$, so $a\cdot c\leq b\cdot c$. $\blacksquare$

***
Definitions used:
- [[Real Numbers]]

Theorems used:
- [[Multiplications with Ring Zeros]]