**Theorem.**
1. There does not exist $n\in \mathbb{N}$ such that $0<n<1$.
2. Let $n\in \mathbb{N}$. Then, there does not exist $m\in \mathbb{N}$ such that $n<m<n+1$.
3. Suppose $m,n\in \mathbb{N}$, and suppose that $m<n+1$. Then, $m\leq n$.

**Proof of First Statement.** For the sake of negation, assume that there is $n\in \mathbb{N}$ such that $0<n<1$. By [[Normal Forms of Natural Numbers]], $n=0$ or $n=k+1$ for some $k\in \mathbb{N}$. We proceed by cases; in each case we will show a contradiction.
- **Case** $n=0$. Since $0<n<1$, we have $n<0$, so $0<0$. However, by reflexivity $0=0$. This contradicts the fact that $<$ is trichotomous.
- **Case** $\exists k\in \mathbb{N} \ (n=k+1)$. Let $k_{0}\in \mathbb{N}$ be such that $n=k_{0}+1$. Since $0<n<1$, we have $n<1$, so $k_{0}+1<1=0+1$. By [[Cancellation Properties on Orders Between Real Numbers]], this means $k_{0}<0$. However, by [[Zero as Smallest Natural Number]], $0\leq k_{0}$. This again contradicts the fact that $<$ is trichotomous.

Since in each case we obtain a contradiction, the assumption that $0<n<1$ must be false. Therefore, $\neg(0<n<1)$. $\blacksquare$

**Proof of Second Statement.** Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(x):\equiv \neg(\exists m\in \mathbb{N} \ (x<m<x+1)).$$To prove the statement, it is enough to show that $\varphi(x)$ is true when $x=n$. We will show by [[Principle of Mathematical Induction]] that $\varphi(x)$ is actually true for all $x\in \mathbb{N}$.
- **Base Case.** By the first statement, there does not exist $m\in \mathbb{N}$ such that $0<m<1$. Therefore, $\varphi(0)$ is true.
- **Induction Step.** Suppose $x\in \mathbb{N}$, and suppose that $\varphi(x)$ is true. For the sake of negation, suppose that there is $m\in \mathbb{N}$ such that $x+1<m<x+2$. By [[Normal Forms of Natural Numbers]], $m=0$ or $m=k+1$ for some $k\in \mathbb{N}$. We proceed by cases; in each case we will show a contradiction.
	- **Case** $m=0$. This means $x+1<0$. However, by [[Zero as Smallest Natural Number]] $0\leq x+1$. This contradicts the fact that $<$ is trichotomous.
	- **Case** $\exists k\in \mathbb{N} \ (m=k+1)$. Let $k_{0}\in \mathbb{N}$ be such that $m=k_{0}+1$. This means $x+1<k_{0}+1<x+2$, so by [[Cancellation Properties on Orders Between Real Numbers]] $x<k_{0}<x+1$. This contradicts the fact that $\varphi(x)$ is true.

	Since in each case we obtain a contradiction, the assumption that there is $m\in \mathbb{N}$ such that $x+1<m<x+2$ must be false. Therefore, there is no $m\in \mathbb{N}$ such that $x+1<m<x+2$, so $\varphi(x+1)$ is also true. $\blacksquare$

**Proof of Third Statement.** By trichotomy of $<$, we have $m<n$, $m=n$, or $n<m$. To show that $m\leq n$, it is then enough to show that $\neg(n<m)$. To do this, assume for the sake of negation that $n<m$. Then, since $m<n+1$, we have $n<m<n+1$. This contradicts the second statement. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]
- [[Real Numbers]]
- [[Subtraction Notation on Rings]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Zero as Smallest Natural Number]]
- [[Normal Forms of Natural Numbers]]
- [[Cancellation Properties on Orders Between Real Numbers]]