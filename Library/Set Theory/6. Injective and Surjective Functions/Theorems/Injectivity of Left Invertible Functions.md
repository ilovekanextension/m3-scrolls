**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Suppose there is $g:B\to A$ such that $g\circ f=\text{id}_{A}$. Then, $f$ is injective.

**Proof.** Suppose $a,b\in A$, and suppose that $f(a)=f(b)$. Then, $g(f(a))=g(f(b))$, so by [[Evaluations of Composite Functions]] $g\circ f(a)=g\circ f(b)$. Since $g\circ f=\text{id}_{A}$, we have $\text{id}_{A}(a)=\text{id}_{A}(b)$. Therefore, $a=b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Injective Function]]

Theorems used:
- [[Evaluations of Composite Functions]]