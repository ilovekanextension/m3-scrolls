Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. An object $b\in B$ is called a **greatest object** of $B$ (under $\leq$) if for all $x\in B$ we have $x\leq b$.

**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $b$ and $c$ are both greatest objects of $B$. Then, $b=c$.

**Proof.** Since $b$ is a greatest object of $B$ and $c\in B$, we have $c\leq b$. Since $c$ is also a greatest object of $B$ and $b\in B$, we have $b\leq c$. By antisymmetry, we therefore have $b=c$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Partial Order]]