**Definition.** Let $A$ be a set. Let $f:A\to A$. Suppose $B\subseteq A$. The smallest object (under $\subseteq$) of the set $$\{X\subseteq A\mid B\subseteq X\wedge \forall x\in X \ (f(x)\in X)\}$$of all sets containing $B$ that's closed under $f$ is called the **closure** of $B$ under $f$. That is, the closure of $B$ under $f$ is the set $C\subseteq A$ satisfying the following properties:
- $B\subseteq C$.
- $C$ is closed under $f$.
- For all sets $X\subseteq A$, if $B\subseteq X$ and $X$ is closed under $f$, then $C\subseteq X$.

***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Function]]
- [[Closed Subset]]
- [[Smallest Object]]