**Theorem.** Let $a,b,c,d\in \mathbb{R}$.
1. Suppose $a<b$ and $c<d$. Then, $a+c<b+d$.
2. Suppose $a<b$ and $c<0$. Then, $a\cdot c>b\cdot c$.
3. Suppose $a>1$. Then, $a\cdot a>a$.
4. Suppose $0<a<1$. Then, $a\cdot a<a$.
5. Suppose $0\leq a<b$ and $0\leq c<d$. Then, $a\cdot c<b\cdot d$.

**Proof of First Statement.** Since $a<b$, we have $a+c<b+c$. Likewise, since $c<d$ we have $b+c<b+d$. Therefore, by transitivity of $<$ we have $a+c<b+d$. $\blacksquare$

**Proof of Second Statement.** Since $c<0$, by [[Orders Between Additive and Multiplicative Inverses]] $-0<-c$, so by [[Inverses of Group Identities]] $0<-c$. We then have $a\cdot(-c)<b\cdot(-c)$. By [[Multiplications with Additive Inverses]], this means $-(a\cdot c)<-(b\cdot c)$, so by [[Orders Between Additive and Multiplicative Inverses]] and [[Involution Property on Group Inverses]] we have $b\cdot c<a\cdot c$. $\blacksquare$

**Proof of Third Statement.** By [[Positivity of Squares of Real Numbers]], $1>0$. Since $a>1$, by transitivity of $<$ we have $a>0$. Therefore, since $a>1$, we have $a\cdot a>a\cdot 1$, so $a\cdot a>a$. $\blacksquare$

**Proof of Fourth Statement.** Since $a<1$ and $0<a$, we have $a\cdot a<1\cdot a$, so $a\cdot a<a$. $\blacksquare$

**Proof of Fifth Statement.** Since $0\leq a$, by definition $0<a$ or $0=a$. Likewise, since $0\leq c$, by definition $0<c$ or $0=c$. We proceed by cases on the first disjunction; in each case we will show that $a\cdot c<b\cdot d$.
- **Case** $0<a$. By transitivity of $<$, this means $0<b$. Since $c<d$, we have $b\cdot c<b\cdot d$. Now, if $0<c$, then since $a<b$ we have $a\cdot c<b\cdot c$, so by transitivity of $<$ we have $a\cdot c<b\cdot d$. If instead $0=c$, then by [[Multiplications with Ring Zeros]] $$a\cdot c=a\cdot 0=0=b\cdot 0=b\cdot c,$$so since $b\cdot c<b\cdot d$ we have $a\cdot c<b\cdot d$.
- **Case** $0=a$. Since $a<b$, this means $0<b$. If $0<c$, then by transitivity of $<$, since $c<d$ we have $0<b\cdot d$. In turn, by [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]] $0<b\cdot d$ and therefore, by [[Multiplications with Ring Zeros]], $$a\cdot c=0\cdot c=0<b\cdot d.$$If $0=c$, then $0<d$, so by a similar reasoning $0<b\cdot d$ and therefore $a\cdot c<b\cdot d$. $\blacksquare$

***
Definitions used:
- [[Real Numbers]]

Theorems used:
- [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]]
- [[Positivity of Squares of Real Numbers]]
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Inverses of Group Identities]]
- [[Involution Property on Group Inverses]]
- [[Multiplications with Ring Zeros]]
- [[Multiplications with Additive Inverses]]