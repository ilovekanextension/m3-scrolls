**Theorem.** Let $R$ be an integral domain. Suppose $a,b\in R$. Then, $(a)=(b)$ if and only if there is a unit $u\in R$ such that $a=b\cdot u$.

**Proof of Forward Implication.** Suppose $(a)=(b)$. Since $a\in(a)$, we have $a\in(b)$, so there is $x\in R$ such that $a=b\cdot x$. Likewise, since $b\in(b)$, we also have $b\in(a)$, so there is $y\in R$ such that $b=a\cdot y$. This means $$b=b\cdot x\cdot y,$$so $b\cdot(x\cdot y-1)=0$. Since $R$ is an integral domain, this means $b=0$ or $x\cdot y-1=0$. We proceed by cases; in each case we will show that there is a unit $u\in R$ such that $a=b\cdot u$.
- **Case** $b=0$. By [[Multiplications with Ring Zeros]], this means $a=0\cdot x=0$. Therefore, $a=b$. Clearly $1$ is a unit. We have $$a=b\cdot 1.$$
- **Case** $x\cdot y-1=0$. This means $x\cdot y=1$. Since $R$ is an integral domain, it is commutative, so $y\cdot x=1$. Therefore, $x$ is a unit. $\blacksquare$

**Proof of Backward Implication.** Suppose there is a unit $u\in R$ such that $a=b\cdot u$.

First suppose $x\in(a)$. Then, there is $k\in R$ such that $x=k\cdot a$. Thus, $$x=k\cdot b\cdot u=(k\cdot u)\cdot b,$$so $x\in(b)$. Now suppose $x\in(b)$. Then, there is $k\in R$ such that $x=k\cdot b$. Thus, $$x=k\cdot a\cdot u^{-1}=(k\cdot u^{-1})\cdot a,$$so $x\in(a)$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Principal Ideal]]
- [[Integral Domain]]
- [[Unit]]

Theorems used:
- [[Multiplications with Ring Zeros]]