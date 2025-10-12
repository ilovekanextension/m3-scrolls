**Theorem.** Let $A$, $B$, and $C$ be posets. Let $f:A\to B$ and $g:B\to C$ be monotone functions. Then, $g\circ f$ is also a monotone function.

**Proof.** Suppose $a,b\in A$, and suppose that $a\leq b$. Since $f$ is monotone, we have $f(a)\leq f(b)$. Since $g$ is also monotone, we have $g(f(a))\leq g(f(b))$. By [[Evaluations of Composite Functions]], this means $g\circ f(a)\leq g\circ f(b)$. $\blacksquare$
***
Definitions used:
- [[Poset]]
- [[Monotone Function]]
- [[Composition of Functions]]

Theorems used:
- [[Evaluations of Composite Functions]]