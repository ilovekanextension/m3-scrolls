**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Suppose there is $g:B\to A$ such that $f\circ g=\text{id}_{B}$. Then, $f$ is surjective.

**Proof.** Suppose $b\in B$. By [[Evaluations of Composite Functions]], we have $f(g(b))=f\circ g(b)$. Since $f\circ g=\text{id}_{B}$, we have $f(g(b))=\text{id}_{B}(b)$, so $f(g(b))=b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Surjective Function]]

Theorems used:
- [[Evaluations of Composite Functions]]