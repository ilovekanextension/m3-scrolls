Let $A$ be a set. We say that $A$ is **empty** if for all objects $x$, we have $x\notin A$.

**Theorem.** Let $A$ and $B$ be sets, and suppose that $A$ and $B$ are both empty. Then, $A=B$.

**Proof.** We will show that $A\subseteq B$ and $B\subseteq A$.
- **First Statement.** Suppose $x\in A$. Since $A$ is empty, we have $x\notin A$. Therefore, by explosion $x\in B$. $\blacksquare$
- **Second Statement.** Suppose $x\in B$. Since $B$ is empty, we have $x\notin B$. Therefore, by explosion $x\in A$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Subset]]