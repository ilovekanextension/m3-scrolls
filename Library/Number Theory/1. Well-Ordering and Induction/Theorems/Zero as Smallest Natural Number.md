**Theorem.**
1. $0$ is the smallest object in $\mathbb{N}$.
2. $\mathbb{N}$ is bounded below.

**Proof of First Statement.** Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(n):\equiv 0\leq n.$$To show that $0$ is the smallest natural number, it is enough to show that $\varphi(n)$ is true for all $n\in \mathbb{N}$. To do this, we use [[Principle of Mathematical Induction]].
- **Base Case.** Since $\leq$ is a total order, it is reflexive, so for all $x\in \mathbb{R}$ we have $x\leq x$. In particular, since $0\in \mathbb{N}$ and $\mathbb{N}\subseteq \mathbb{R}$, we have $0\leq 0$. This means $\varphi(0)$ is true.
- **Induction Step.** Suppose $n\in \mathbb{N}$, and suppose that $\varphi(n)$ is true. Then, $0\leq n$. By [[Positivity of Squares of Real Numbers]], $0\leq 1$, so by [[Preservation of Total Orders Under Addition and Multiplication]] $0+0\leq n+1$. This means $0\leq n+1$, so $\varphi(n+1)$ is also true. $\blacksquare$

**Proof of Second Statement.** By [[Smallest Objects as Infima]], since $0$ is the smallest object of $\mathbb{N}$, $0$ is also the infimum of $\mathbb{N}$, so $\mathbb{N}$ is bounded below. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]
- [[Subset]]
- [[Real Numbers]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Positivity of Squares of Real Numbers]]
- [[Preservation of Total Orders Under Addition and Multiplication]]
- [[Smallest Objects as Infima]]