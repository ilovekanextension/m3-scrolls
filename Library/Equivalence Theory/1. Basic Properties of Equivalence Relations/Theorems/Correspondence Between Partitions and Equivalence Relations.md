**Theorem.** Let $A$ be a set. Let $E$ and $P$ be the set of all equivalence relations on $A$ and partitions of $A$ respectively. Then, $E\cong P$.

**Proof.** By [[Quotient Sets as Partitions]], we can define a function $f:E\to P$ as follows: $$f({\sim})=A/{\sim}.$$We will show that $f$ is bijective.
- **Injectivity.** Suppose ${\sim}\in E$ and ${\simeq}\in E$, and suppose that $f(\sim)=f(\simeq)$. Then, $A/{\sim}=A/{\simeq}$. By [[Injectivity of Quotient Sets]], $\sim$ is equal to $\simeq$.
- **Surjectivity.** Suppose $F\in P$. By [[Partitions as Quotient Sets]], there is ${\sim}\in E$ such that $A/{\sim}=F$ or $f(\sim)=F$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Equivalence Relation]]
- [[Quotient Set]]
- [[Partition of Set]]

Theorems used:
- [[Quotient Sets as Partitions]]
- [[Injectivity of Quotient Sets]]
- [[Partitions as Quotient Sets]]