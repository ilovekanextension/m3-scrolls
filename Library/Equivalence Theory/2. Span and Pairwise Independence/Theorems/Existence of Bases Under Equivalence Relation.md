**Theorem.** Let $A$ be a set. Let $\sim$ be an equivalence relation on $A$. Then, assuming Choice, there is a set $B\subseteq A$ such that $B$ is a basis for $A$ under $\sim$.

**Proof.** By Choice, there is $f:A/{\sim}\to A$ such that for all $X\in A/{\sim}$, $f(X)\in X$. We will show that $$f[A/{\sim}]=\{f(X)\in A\mid X\in A/{\sim}\}$$is a basis for $A$.
- **Span.** Suppose $a\in A$. Then, $[a]_{\sim}\in A/{\sim}$, so $f([a]_{\sim})\in f[A/{\sim}]$. By definition of $f$, $f([a]_{\sim})\in[a]_{\sim}$, so $a\sim f([a]_{\sim})$.
- **Pairwise Independence.** Suppose $a,b\in f[A/{\sim}]$, and suppose that $a\sim b$. Since $a,b\in f[A/{\sim}]$, there are $x,y\in A$ such that $a=f([x]_{\sim})$ and $b=f([y]_{\sim})$. By definition of $f$, $a\in[x]_{\sim}$ and $b\in[y]_{\sim}$, so $a\sim x$ and $b\sim y$. Since $a\sim b$, by symmetry and transitivity $x\sim y$, so by [[Properties of Membership and Equality of Equivalence Classes]] $[x]_{\sim}=[y]_{\sim}$. Therefore, $f([x]_{\sim})=f([y]_{\sim})$, so $a=b$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Spanning Set]]
- [[Pairwise Independent Set]]
- [[Basis Under Equivalence Relation]]
- [[Function]]
- [[Image of Subset]]

Theorems used:
- [[Properties of Membership and Equality of Equivalence Classes]]