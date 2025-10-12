**Theorem.** Let $A$ be a set.
1. Let $f:A\to A$. Suppose $B\subseteq A$. Then, $B$ is closed under $f$ if and only if the closure of $B$ under $f$ is itself.
2. Let $\circ:A\times A\to A$. Suppose $B\subseteq A$. Then, $B$ is closed under $\circ$ if and only if the closure of $B$ under $\circ$ is itself.

**Proof of First Statement.** First suppose $B$ is closed under $f$. We will show that the closure of $B$ under $f$ is itself.
- By [[Subset Relation as Partial Order]], $B\subseteq B$.
- By assumption, $B$ is closed under $f$.
- Suppose $X\subseteq A$. Suppose $B\subseteq X$ and $X$ is closed under $f$. Then, $B\subseteq X$.

Now suppose that the closure of $B$ under $f$ is itself. Then, by definition $B$ is closed under $f$. $\blacksquare$

**Proof of Second Statement.** First suppose $B$ is closed under $\circ$. We will show that the closure of $B$ under $\circ$ is itself.
- By [[Subset Relation as Partial Order]], $B\subseteq B$.
- By assumption, $B$ is closed under $\circ$.
- Suppose $X\subseteq A$. Suppose $B\subseteq X$ and $X$ is closed under $\circ$. Then, $B\subseteq X$.

Now suppose that the closure of $B$ under $\circ$ is itself. Then, by definition $B$ is closed under $\circ$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Function]]
- [[Closed Subset]]
- [[Closure of Subset]]

Theorems used:
- [[Subset Relation as Partial Order]]