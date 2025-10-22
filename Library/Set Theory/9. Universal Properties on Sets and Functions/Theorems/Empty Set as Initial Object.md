**Theorem.** Let $A$ be a set. Then, $A$ is empty if and only if for all sets $X$ there is a unique function $A\to X$.

**Proof of Forward Implication.** Suppose $A$ is empty. Suppose $X$ is a set.
- **Existence.** The empty relation $\varnothing\subseteq A\times X$ is a function.
- **Uniqueness.** Suppose $f:A\to X$ and $g:A\to X$. Suppose $a\in A$. Since $A$ is empty, $a\notin A$, so by explosion we can conclude that $f(a)=g(a)$. Therefore, by [[Extensionality of Functions]] $f=g$. $\blacksquare$

**Proof of Backward Implication.** Suppose that for all sets $X$ there is a unique function $A\to X$. To show that $A$ is empty, we will show that $A=\varnothing$. By [[Empty Set as Subset of Any Set]], it is therefore enough to show that $A\subseteq \varnothing$.

Suppose $a\in A$. Since for all sets $X$ there is a unique function $A\to X$, in particular there is a unique function $A\to\varnothing$. We can therefore construct a function $f:A\to\varnothing$. Since $a\in A$, we have $f(a)\in\varnothing$. Since $\varnothing$ is empty, $f(a)\notin \varnothing$, so by explosion $a\in\varnothing$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Empty Set]]
- [[Relation]]
- [[Function]]

Theorems used:
- [[Empty Set as Subset of Any Set]]
- [[Extensionality of Functions]]