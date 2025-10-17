**Theorem.** Let $S$ and $T$ be subsets of $\mathbb{R}$.
1. Suppose $u\in \mathbb{R}$, and suppose that $u$ is an upper bound for $S$. Then, $-u$ is a lower bound for $-S$.
2. Suppose $\ell\in \mathbb{R}$, and suppose that $\ell$ is a lower bound for $S$. Then, $-\ell$ is an upper bound for $-S$.
3. Suppose $u\in \mathbb{R}$ and $v\in \mathbb{R}$, and suppose that $u$ and $v$ are upper bounds for $S$ and $T$ respectively. Then, $u+v$ is an upper bound for $S+T$.
4. Suppose $u\in \mathbb{R}$ and $v\in \mathbb{R}$, and suppose that $u$ and $v$ are lower bounds for $S$ and $T$ respectively. Then, $u+v$ is a lower bound for $S+T$.

**Proof of First Statement.** Suppose $x\in-S$. Then, there is $z\in S$ such that $x=-z$. Since $u$ is an upper bound for $S$ and $z\in S$, we have $z\leq u$, so by [[Orders Between Additive and Multiplicative Inverses]] $-u\leq-z$. Therefore, $-u\leq x$. $\blacksquare$

**Proof of Second Statement.** Suppose $x\in-S$. Then, there is $z\in S$ such that $x=-z$. Since $\ell$ is a lower bound for $S$ and $z\in S$, we have $\ell\leq z$, so by [[Orders Between Additive and Multiplicative Inverses]] $-z\leq-\ell$. Therefore, $x\leq-\ell$. $\blacksquare$

**Proof of Third Statement.** Suppose $a\in S+T$. Then, there is $x\in S$ and $y\in T$ such that $a=x+y$. Since $u$ is an upper bound for $S$ and $x\in S$, we have $x\leq u$. Likewise, since $v$ is an upper bound for $T$ and $y\in T$, we have $y\leq v$. By [[Preservation of Total Orders Under Addition and Multiplication]], we then have $x+y\leq u+v$, so $a\leq u+v$. $\blacksquare$

**Proof of Fourth Statement.** Suppose $a\in S+T$. Then, there is $x\in S$ and $y\in T$ such that $a=x+y$. Since $u$ is a lower bound for $S$ and $x\in S$, we have $u\leq x$. Likewise, since $v$ is a lower bound for $T$ and $y\in T$, we have $v\leq y$. By [[Preservation of Total Orders Under Addition and Multiplication]], we then have $u+v\leq x+y$, so $u+v\leq a$. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Upper Bound]]
- [[Lower Bound]]
- [[Arithmetic Operations on Subsets of Ring]]

Theorems used:
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Preservation of Total Orders Under Addition and Multiplication]]