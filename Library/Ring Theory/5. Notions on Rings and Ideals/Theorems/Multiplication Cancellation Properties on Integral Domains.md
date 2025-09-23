**Theorem.** Let $R$ be an integral domain. Suppose $a,b,c\in R$, and suppose that $a$ is nonzero.
1. Suppose $a\cdot b=a\cdot c$. Then, $b=c$.
2. Suppose $b\cdot a=c\cdot a$. Then, $b=c$.

**Proof of First Statement.** Since $a\cdot b=a\cdot c$, we have $a\cdot b-a\cdot c=0$, so $a\cdot(b-c)=0$. Since $R$ is an integral domain, $a=0$ or $b-c=0$. Since $a$ is nonzero, we cannot have $a=0$, so $b-c=0$. By [[Cancellation Properties on Groups]], this means $b=c$. $\blacksquare$

**Proof of Second Statement.** Since $R$ is an integral domain, $R$ is commutative, so $a\cdot b=a\cdot c$. By the first statement, this means $b=c$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Subtraction Notation on Rings]]
- [[Integral Domain]]

Theorems used:
- [[Cancellation Properties on Groups]]