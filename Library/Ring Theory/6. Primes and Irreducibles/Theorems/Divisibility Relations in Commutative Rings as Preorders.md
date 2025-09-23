**Theorem.** Let $R$ be a commutative ring.
1. For all $a\in R$, $a\mid a$.
2. For all $a,b,c\in R$, if $a\mid b$ and $b\mid c$, then $a\mid c$.

**Proof of First Statement.** Suppose $a\in R$. We have $$a=1\cdot a,$$so $a\mid a$. $\blacksquare$

**Proof of Second Statement.** Suppose $a,b,c\in R$, and suppose that $a\mid b$ and $b\mid c$. Since $a\mid b$, there is $k\in R$ such that $b=k\cdot a$. Since $b\mid c$, there is $l\in R$ such that $c=l\cdot b$. We then have $$c=l\cdot b=l\cdot(k\cdot a)=(l\cdot k)\cdot a,$$so $a\mid c$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Divisor]]