**Theorem.** Let $R$ be a nontrivial commutative ring. Then, $R$ is a field if and only if for all ideals $I$ of $R$, we have $I=(0)$ or $I=(1)$.

**Proof of Forward Implication.** Suppose $R$ is a field. Suppose $I$ is an ideal of $R$. Either $1\in I$ or $1\notin I$. We proceed by cases; in each case we will show that $I=(0)$ or $I=(1)$.
- **Case** $1\in I$. We will show that $I=(1)$. By [[Special Ideals as Principal Ideals]], $(1)=R$, so $I\subseteq(1)$. Now suppose $x\in(1)$. Since $1\in I$, we have $$x=x\cdot 1\in I.$$
- **Case** $1\notin I$. We will show that $I=(0)$. First suppose $x\in I$. By [[Special Ideals as Principal Ideals]], to show that $x\in(0)$ it is enough to show that $x\in\{0\}$, which means it is enough to show that $x=0$. For the sake of contradiction, assume that $x\neq 0$. Then, $x$ has a multiplicative inverse $x^{-1}\in R$. Since $I$ is an ideal and $x\in I$, we have $$1=x\cdot x^{-1}\in I.$$This contradicts the fact that $1\notin I$. Therefore, the assumption that $x\neq 0$ is false, so $x=0$. Now suppose $x\in(0)$. Then, $x=0$. Since $I$ is an ideal, $I$ is a subgroup, so $0\in I$. Therefore, $x\in I$. $\blacksquare$

**Proof of Backward Implication.** Suppose that for all ideals $I$ of $R$, we have $I=(0)$ or $I=(1)$. Suppose $x\in R$ is nonzero. Consider the principal ideal $(x)$. Since $x$ is nonzero, we have $x\notin\{0\}$, so by [[Special Ideals as Principal Ideals]] $x\notin(0)$. We have $x\in(x)$, so this means $(x)\neq(0)$. Therefore, by assumption we must have $(x)=(1)$. Since $1\in(1)$, we have $1\in(x)$, so there is $y\in R$ such that $x\cdot y=1$. Since $R$ is commutative, we also have $y\cdot x=1$. Therefore, $y$ is the multiplicative inverse of $x$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Ideal]]
- [[Field]]
- [[Principal Ideal]]

Theorems used:
- [[Special Ideals as Principal Ideals]]