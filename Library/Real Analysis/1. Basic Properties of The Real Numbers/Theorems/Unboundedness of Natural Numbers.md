**Theorem.** $\mathbb{N}$ is not bounded above.

**Proof.** For the sake of negation, assume that $\mathbb{N}$ is bounded above. Then, since $\mathbb{N}$ is nonempty (by definition, $0\in \mathbb{N}$), by the completeness property of real numbers $\mathbb{N}$ has a supremum $\sup(\mathbb{N})$. By [[Positivity of Squares of Real Numbers]], $1>0$, so by [[Criterion for Upper Bounds as Suprema]] there is $n\in \mathbb{N}$ such that $\sup(\mathbb{N})-1<n$. This means $$\sup(\mathbb{N})=\sup(\mathbb{N})-1+1<n+1.$$By definition of $\mathbb{N}$, since $n\in \mathbb{N}$, we must have $n+1\in \mathbb{N}$. This contradicts the fact that $\sup(\mathbb{N})$ is an upper bound for $\mathbb{N}$: since $n+1\in \mathbb{N}$, we must have $n+1\leq \sup(\mathbb{N})$, but this violates trichotomy of $<$. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Natural Numbers]]
- [[Supremum]]
- [[Nonempty Set]]

Theorems used:
- [[Positivity of Squares of Real Numbers]]
- [[Criterion for Upper Bounds as Suprema]]