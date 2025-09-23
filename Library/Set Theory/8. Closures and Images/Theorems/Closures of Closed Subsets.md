**Theorem.** Let $A$ be a set. Let $f:A\to A$. Suppose $B\subseteq A$. Then, $B$ is closed under $f$ if and only if the closure of $B$ under $f$ is itself.

**Proof of Forward Implication.** Suppose $B$ is closed under $f$.
- By [[Subset Relation as Partial Order]], $B\subseteq B$.
- By assumption, $B$ is closed under $f$.
- Suppose $X\subseteq A$. Suppose $B\subseteq X$ and $X$ is closed under $f$. Then, $B\subseteq X$. $\blacksquare$

**Proof of Backward Implication.** Suppose the closure of $B$ under $f$ is itself. Then, by definition $B$ is closed under $f$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Function]]
- [[Closed Subset]]
- [[Closure of Subset]]

Theorems used:
- [[Subset Relation as Partial Order]]