**Theorem.** Let $A$ be a set. Then, $A$ is a singleton set if and only if for all sets $X$ there is a unique function $X\to A$. Hence, in $\mathsf{Set}$ terminal objects are precisely singleton sets.

**Proof of Forward Implication.** Suppose $A$ is a singleton set. Then, there is an object $*$ such that $A=\{*\}$. Suppose $X$ is a set.
- **Existence.** We can construct a function $f:X\to A$ defined as $f(x)=*$.
- **Uniqueness.** Suppose $g:X\to A$. Suppose $x\in X$. Then, $g(x)\in A$. Since $A=\{*\}$, we must have $g(x)=*$. We also have $f(x)=*$, so by [[Extensionality of Functions]] $g=f$. $\blacksquare$

**Proof of Backward Implication.** Suppose that for all sets $X$ there is a unique function $f:X\to A$. Then, in particular there is a unique function $\{*\}\to A$. To show that $A$ is a singleton, we will show that for all $a,b\in A$, we have $a=b$.

Suppose $a,b\in A$. We can construct functions $f:\{*\}\to A$ and $g:\{*\}\to A$ defined as $$f(*)=a\wedge g(*)=b.$$Since there is a unique function $\{*\}\to A$, we must have $f=g$. Therefore, by [[Extensionality of Functions]] we have $f(*)=g(*)$. This means $a=b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Enumeration Notation]]
- [[Function]]

Theorems used:
- [[Extensionality of Functions]]