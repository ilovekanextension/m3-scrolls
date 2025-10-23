**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$ be bijective.
1. $f^{-1}\circ f=\text{id}_{A}$.
2. $f\circ f^{-1}=\text{id}_{B}$.

**Proof of First Statement.** Suppose $a\in A$. Define $c\in B$ as the object such that $f^{-1}(f(a))=c$. Then, by [[Values of Inverse Functions]], $f(c)=f(a)$. Since $f$ is bijective, it is injective, so $c=a$. This means $f^{-1}(f(a))=a=\text{id}_{A}(a)$, so by [[Evaluations of Composite Functions]] $$f^{-1}\circ f(a)=\text{id}_{A}(a).$$Therefore, by [[Extensionality of Functions]] $f^{-1}\circ f=\text{id}_{A}$. $\blacksquare$

**Proof of Second Statement.** Suppose $b\in B$. Since $f$ is bijective, it is surjective, so there is $a\in A$ such that $f(a)=b$. By [[Values of Inverse Functions]], we then have $f^{-1}(b)=a$, so $f(f^{-1}(b))=f(a)=b$. By [[Evaluations of Composite Functions]], this means $$f\circ f^{-1}(b)=\text{id}_{B}(b),$$so by [[Extensionality of Functions]] $f\circ f^{-1}=\text{id}_{B}$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Injective Function]]
- [[Surjective Function]]
- [[Bijective Function]]
- [[Inverse of Bijective Function]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Values of Inverse Functions]]