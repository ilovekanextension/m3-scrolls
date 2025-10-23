**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Then, $f$ is an epimorphism if and only if $f$ is surjective.

**Proof of Forward Implication.** Suppose $f$ is an epimorphism. Suppose $b\in B$. Define a set $S=\{0,1\}$ and functions $s:B\to S$ and $t:B\to S$ as follows: for all $x\in B$, $$s(x)=0 \wedge t(x)=\begin{cases}
0, & x\in f[A] \\
1, & x\notin f[A].
\end{cases}$$We will first show that $s\circ f=t\circ f$.
Suppose $a\in A$. By definition, $f(a)\in f[A]$, so $t(f(a))=0$. By definition of $s$, we also have $s(f(a))=0$, so $s(f(a))=t(f(a))$. By [[Evaluations of Composite Functions]], we then have $s\circ f(a)=t\circ f(a)$. By [[Extensionality of Functions]], this shows that $s\circ f=t\circ f$.

Since $f$ is an epimorphism, we must have $s=t$, so by [[Extensionality of Functions]] again $s(b)=t(b)$. Since $s(b)=0$ by definition of $s$, we must have $t(b)=0$, so $b\in f[A]$. This means there is $a\in A$ such that $b=f(a)$. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is surjective. Suppose $X$ is a set, and suppose that $s:B\to X$ and $t:B\to X$ satisfy $s\circ f=t\circ f$. Suppose $b\in B$. Since $f$ is surjective, there is $a\in A$ such that $f(a)=b$. Since $s\circ f=t\circ f$, by [[Extensionality of Functions]] $s\circ f(a)=t\circ f(a)$, so by [[Evaluations of Composite Functions]] $s(f(a))=t(f(a))$. Therefore, $s(b)=t(b)$, so by [[Extensionality of Functions]] we can conclude that $s=t$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Category of Sets]]
- [[Composition of Functions]]
- [[Surjective Function]]
- [[Epimorphism]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]