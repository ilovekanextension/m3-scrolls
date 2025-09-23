**Theorem.** Let $R$ be a commutative ring. Suppose $a\in R$. Then, the set $$I=\{r\cdot a\in R\mid r\in R\}$$is an ideal of $R$.

**Proof.** We first show that $I$ is a subgroup of $R$.
- **Closure Under Identity.** By [[Multiplications with Ring Zeros]], $0=0\cdot a\in I$.
- **Closure Under Composition.** Suppose $x,y\in I$. Then, there are $r,s\in R$ such that $x=r\cdot a$ and $y=s\cdot a$. We have $$x+y=r\cdot a+s\cdot a=(r+s)\cdot a\in I.$$
- **Closure Under Inverses.** Suppose $x\in I$. Then, there is $r\in R$ such that $x=r\cdot a$. By [[Multiplications with Additive Inverses]], $$-x=-(r\cdot a)=-r\cdot a\in I.$$

We now show that for all $r\in R$ and $x\in I$, $r\cdot x\in I$ and $x\cdot r\in I$. Suppose $r\in R$ and $x\in I$. Since $x\in I$, there is $s\in R$ such that $x=s\cdot a$. We then have $$r\cdot x=r\cdot (s\cdot a)=(r\cdot s)\cdot a\in I.$$Since $R$ is commutative, $r\cdot x=x\cdot r$, so $x\cdot r\in I$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Ideal]]
- [[Enumeration Notation]]
- [[Subgroup]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Multiplications with Additive Inverses]]