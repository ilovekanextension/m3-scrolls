**Theorem.** Let $a,b,c,d\in \mathbb{R}$.
1. Suppose $a\leq b$ and $c<d$. Then, $a+c\leq b+d$.
2. Suppose $a\leq b$ and $c\leq 0$. Then, $a\cdot c\geq b\cdot c$.
3. Suppose $a\geq1$. Then, $a\cdot a\geq a$.
4. Suppose $0\leq a\leq 1$. Then, $a\cdot a\leq a$.
5. Suppose $0\leq a\leq b$ and $0\leq c\leq d$. Then, $a\cdot c\leq b\cdot d$.

**Proof of First Statement.** By [[Basic Order Properties for Total Order on Real Numbers]], since $a\leq b$ we have $a+c\leq b+c$. Likewise, since $c\leq d$ we have $b+c\leq b+d$. Therefore, by transitivity of $\leq$ we have $a+c\leq b+d$. $\blacksquare$

**Proof of Second Statement.** Since $c\leq 0$, by [[Orders Between Additive and Multiplicative Inverses]] $-0\leq -c$, so by [[Inverses of Group Identities]] $0\leq -c$. By [[Basic Order Properties for Total Order on Real Numbers]], we then have $a\cdot(-c)\leq b\cdot(-c)$. By [[Multiplications with Additive Inverses]], this means $-(a\cdot c)\leq -(b\cdot c)$, so by [[Orders Between Additive and Multiplicative Inverses]] and [[Involution Property on Group Inverses]] we have $b\cdot c\leq a\cdot c$. $\blacksquare$

**Proof of Third Statement.** By [[Positivity of Squares of Real Numbers]], $1\geq 0$. Since $a\geq 1$, by transitivity of $\leq$ we have $a\geq 0$. Therefore, by [[Basic Order Properties for Total Order on Real Numbers]], since $a\geq 1$ we have $a\cdot a\geq a\cdot 1$, so $a\cdot a\geq a$. $\blacksquare$

**Proof of Fourth Statement.** By [[Basic Order Properties for Total Order on Real Numbers]], since $a\leq 1$ and $0\leq a$, we have $a\cdot a\leq 1\cdot a$, so $a\cdot a\leq a$. $\blacksquare$

**Proof of Fifth Statement.** Since $c\leq d$ and $0\leq b$, by [[Basic Order Properties for Total Order on Real Numbers]] we have $b\cdot c\leq b\cdot d$. Likewise, since $a\leq b$ and $c\leq 0$, we have $a\cdot c\leq b\cdot c$. Therefore, by transitivity of $\leq$ we have $a\cdot c\leq b\cdot d$. $\blacksquare$

***
Definitions used:
- [[Real Numbers]]

Theorems used:
- [[Basic Order Properties for Total Order on Real Numbers]]
- [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]]
- [[Positivity of Squares of Real Numbers]]
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Inverses of Group Identities]]
- [[Involution Property on Group Inverses]]
- [[Multiplications with Ring Zeros]]
- [[Multiplications with Additive Inverses]]