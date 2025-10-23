**Theorem.** Let $A$, $B$, and $C$ be sets. Let $f:A\twoheadrightarrow B$ and $g:B\twoheadrightarrow C$. Then, $g\circ f:A\twoheadrightarrow C$.

**Proof.** Suppose $c\in C$. Since $g$ is surjective, there is $b\in B$ such that $g(b)=c$. Since $f$ is surjective, there is $a\in A$ such that $f(a)=b$. We therefore have $g(f(a))=c$, so by [[Evaluations of Composite Functions]] $g\circ f(a)=c$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Composition of Functions]]
- [[Surjective Function]]

Theorems used:
- [[Evaluations of Composite Functions]]