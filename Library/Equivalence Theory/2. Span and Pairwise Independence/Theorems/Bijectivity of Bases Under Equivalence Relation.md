**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$. Suppose $B$ and $C$ are subsets of $A$, and suppose that $B$ and $C$ are both bases for $A$. Then, $B\cong A$.

**Proof.** Since $B$ is a basis for $A$, by [[Criterion for Bases Under Equivalence Relation]] the function $f:B\to A/{\sim}$ defined as $$f(b)=[b]_{\sim}$$is bijective. Since $C$ is also a basis for $A$, the function $g:C\to A/{\sim}$ defined as $$g(c)=[c]_{\sim}$$is also bijective. By [[Inverses of Bijective Functions as Bijective Functions]] and [[Compositions of Bijective Functions as Bijective Functions]], $g^{-1}:A/{\sim}\to C$ is bijective, so $g^{-1}\circ f:B\to C$ is bijective. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Basis Under Equivalence Relation]]
- [[Function]]
- [[Composition of Functions]]
- [[Inverse of Bijective Function]]
- [[Bijective Function]]

Theorems used:
- [[Criterion for Bases Under Equivalence Relation]]
- [[Inverses of Bijective Functions as Bijective Functions]]
- [[Compositions of Bijective Functions as Bijective Functions]]