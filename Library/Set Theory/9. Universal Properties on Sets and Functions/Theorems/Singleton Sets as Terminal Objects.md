**Theorem.** Let $A$ be a set. Then, $A$ is a terminal object if and only if $A$ is a singleton.

**Proof of Forward Implication.** Suppose that $A$ is a terminal object. Then, for all sets $X$ there is a unique function $f:X\to A$. In particular, letting $*$ be an arbitrary object, there is a unique function $\{*\}\to A$. To show that $A$ is a singleton, we will show that for all $a,b\in A$, we have $a=b$.

Suppose $a,b\in A$. Then, we can construct two functions $f:\{*\}\to A$ and $g:\{*\}\to A$ defined as $$f(*)=a\wedge g(*)=b.$$Since the function $\{*\}\to A$ is unique, we must have $f=g$. Therefore, by [[Extensionality of Functions]] we have $f(*)=g(*)$, so $a=b$. $\blacksquare$

**Proof of Backward Implication.** Suppose $A$ is a singleton set. Then, there is an object $*$ such that $A=\{*\}$. Suppose $X$ is a set.
- **Existence.** We can construct a function $f:X\to A$ defined as $f(x)=*$.
- **Uniqueness.** Suppose $g:X\to A$. Suppose $x\in X$. Then, $g(x)\in A$. Since $A=\{*\}$, we must have $g(x)=*$. Therefore, $$f(x)=*=g(x).$$By [[Extensionality of Functions]], we can conclude that $g=f$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Singleton]]
- [[Function]]
- [[Category of Sets]]
- [[Terminal Object]]

Theorems used:
- [[Extensionality of Functions]]