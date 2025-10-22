**Theorem.** Let $S$ be a nonempty subset of $\mathbb{R}$. Suppose $u\in \mathbb{R}$ is an upper bound for $S$. Then, $u$ is the supremum of $S$ if and only if for all $\varepsilon>0$ there is $x\in S$ such that $u-\varepsilon<x$.

**Proof of Forward Implication.** Suppose $u=\sup(S)$. Suppose $\varepsilon>0$. For the sake of contradiction, assume that for all $x\in S$ we have $\neg(u-\varepsilon<x)$. Then, by trichotomy of $<$, for all $x\in S$ we have $x\leq u-\varepsilon$. This means $u-\varepsilon$ is an upper bound for $S$. Since $u=\sup(S)$, we then must have $$u+0=u\leq u-\varepsilon,$$so by [[Cancellation Properties on Orders Between Real Numbers]] $0\leq-\varepsilon$. By [[Orders Between Additive and Multiplicative Inverses]] and [[Involution Property on Group Inverses]], this means $\varepsilon\leq 0$. However, by assumption $\varepsilon>0$. These contradict the fact that $<$ is trichotomous. $\blacksquare$

**Proof of Backward Implication.** Suppose that for all $\varepsilon>0$ there is $x\in S$ such that $u-\varepsilon<x$. Suppose $v\in \mathbb{R}$ is an upper bound for $S$. We will show that $u\leq v$. To do this, assume for the sake of negation that $\neg(u\leq v)$. Then, by trichotomy of $<$, we must have $v<u$. This means $$0=v-v<u-v,$$so by assumption there is $x\in S$ such that $u-(u-v)<x$. By [[Inverses of Group Compositions]] and [[Involution Property on Group Inverses]], this means $u-u+v<x$, so $v<x$. However, since $v$ is an upper bound for $S$ and $x\in S$, we must have $x\leq v$. This contradicts the fact that $<$ is trichotomous. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Supremum]]

Theorems used:
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Cancellation Properties on Orders Between Real Numbers]]
- [[Involution Property on Group Inverses]]
- [[Inverses of Group Compositions]]