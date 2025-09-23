Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. An object $b\in B$ is called a **smallest object** of $B$ (**under** $\leq$) if for all $x\in B$ we have $b\leq x$.

**Theorem.** Let $A$ be a set. Let $\leq$ be a partial order on $A$. Suppose $B\subseteq A$. Suppose $b$ and $c$ are both smallest objects of $B$. Then, $b=c$.

**Proof.** Since $b$ is a smallest object of $B$ and $c\in B$, we have $b\leq c$. Since $c$ is also a smallest object of $B$ and $b\in B$, we have $c\leq b$. By antisymmetry, we therefore have $b=c$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Partial Order]]