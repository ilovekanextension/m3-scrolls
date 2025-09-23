**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$. Then, $A/{\sim}$ is a partition of $A$. That is, the following statements are true.
1. Suppose $X\in A/{\sim}$. Then, $X$ is nonempty.
2. Suppose $a\in A$. Then, there is a unique class $X\in A/{\sim}$ such that $a\in X$.

**Proof of First Statement.** Since $X\in A/{\sim}$, there is $a\in A$ such that $X=[a]_{\sim}$. By [[Properties of Membership and Equality of Equivalence Classes]],we have $a\in[a]_{\sim}$, so $a\in X$.

**Proof of Second Statement.**
- **Existence.** By [[Properties of Membership and Equality of Equivalence Classes]], $a\in[a]_{\sim}$.
- **Uniqueness.** Suppose $X\in A/{\sim}$, and suppose $a\in X$. Since $X\in A/{\sim}$, there is $b\in A$ such that $X=[b]_{\sim}$. Since $a\in X$, we have $a\in[b]_{\sim}$, so $a\sim b$. By [[Properties of Membership and Equality of Equivalence Classes]], this means $[a]_{\sim}=[b]_{\sim}$, so $X=[a]_{\sim}$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Partition of Set]]

Theorems used:
- [[Properties of Membership and Equality of Equivalence Classes]]