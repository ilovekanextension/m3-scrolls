**Theorem.** Let $A$ be a set. Then, $A$ is an initial object if and only if $A$ is empty.

**Proof of Forward Implication.** Suppose that $A$ is an initial object. Then, for all sets $X$ there is a unique function $f:A\to X$. By [[Empty Set as Subset of Any Set]], $\varnothing\subseteq A$. Therefore, to prove that $A$ is empty, it is enough to show that $A\subseteq\varnothing$.

Suppose $a\in A$. Since for all sets $X$ there is a unique function $A\to X$, in particular there is a unique function $A\to\varnothing$. We can therefore construct a function $f:A\to\varnothing$. Since $a\in A$, we have $f(a)\in\varnothing$. Since $\varnothing$ is empty, $f(a)\notin \varnothing$, so by explosion $a\in\varnothing$. $\blacksquare$

**Proof of Backward Implication.** Suppose $A$ is empty. Suppose $X$ is a set.
- **Existence.** The empty relation $\varnothing\subseteq A\times X$ is a function.
- **Uniqueness.** Suppose $f:A\to X$ and $g:A\to X$. Suppose $a\in A$. Since $A$ is empty, $a\notin A$, so by explosion we can conclude that $f(a)=g(a)$. Therefore, by [[Extensionality of Functions]] $f=g$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Empty Set]]
- [[Relation]]
- [[Function]]
- [[Category of Sets]]
- [[Initial Object]]

Theorems used:
- [[Empty Set as Subset of Any Set]]
- [[Extensionality of Functions]]