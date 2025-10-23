**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$.
1. $f\circ \text{id}_{A}=f$.
2. $\text{id}_{B}\circ f=f$.

**Proof of First Statement.** By [[Evaluations of Composite Functions]], for all $a\in A$ we have $$f\circ \text{id}_{A}(a)=f(\text{id}_{A}(a))=f(a)$$Therefore, by [[Extensionality of Functions]] $f\circ \text{id}_{A}=f$. $\blacksquare$

**Proof of Second Statement.** By [[Evaluations of Composite Functions]], for all $a\in A$ we have $$\text{id}_{B}\circ f(a)=\text{id}_{B}(f(a))=f(a)$$Therefore, by [[Extensionality of Functions]] $\text{id}_{B}\circ f=f$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Identity Function]]
- [[Composition of Functions]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]