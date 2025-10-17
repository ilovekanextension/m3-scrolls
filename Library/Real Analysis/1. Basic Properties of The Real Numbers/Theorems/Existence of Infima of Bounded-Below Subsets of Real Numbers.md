**Theorem.** Let $S$ be a nonempty subset of $\mathbb{R}$, and suppose that $S$ is bounded below. Then, the infimum of $S$ exists. That is, there is $i\in \mathbb{R}$ such that $i=\inf(S)$.

**Proof.** Consider the set $-S$. Since $S$ is nonempty, we can choose $x\in \mathbb{R}$ such that $x\in S$. This means $-x\in -S$, so $-S$ is nonempty. Also, since $S$ is bounded below, there is $s\in \mathbb{R}$ such that $s$ is a lower bound for $S$. By [[Bounds for Subsets Under Arithmetic Operations]], this means $-s$ is an upper bound for $-S$, so $-S$ is bounded above.

Since $-S$ is a nonempty subset of $\mathbb{R}$ that has an upper bound, by the completeness property $-S$ has a supremum $\sup(-S)$. We will now show that $-\sup(-S)$ is the infimum of $S$.
- **Lower Bound Property.** Suppose $x\in S$. Then, by definition $-x\in -S$, so $-x\leq \sup(-S)$. By [[Orders Between Additive and Multiplicative Inverses]], this means $-\sup(-S)\leq x$.
- **Greatest Property.** Suppose $\ell\in \mathbb{R}$, and suppose that $\ell$ is a lower bound for $S$. Then, by [[Bounds for Subsets Under Arithmetic Operations]] $-\ell$ is an upper bound for $-S$. Since $\sup(-S)$ is the smallest upper bound for $-S$, we must have $\sup(-S)\leq -\ell$, so by [[Orders Between Additive and Multiplicative Inverses]] and [[Involution Property on Group Inverses]] $\ell\leq -\sup(-S)$. $\blacksquare$

***
Definitions used:
- [[Real Numbers]]
- [[Supremum]]
- [[Infimum]]
- [[Arithmetic Operations on Subsets of Ring]]

Theorems used:
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Bounds for Subsets Under Arithmetic Operations]]
- [[Involution Property on Group Inverses]]