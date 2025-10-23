**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Then, $f$ is a monomorphism if and only if $f$ is injective.

**Proof of Forward Implication.** Suppose $f$ is a monomorphism. Suppose $a,b\in A$, and suppose that $f(a)=f(b)$. Define a set $S=\{*\}$ and functions $s:S\to A$ and $t:S\to A$ as follows: $$s(*)=a
\wedge t(*)=b.$$Since $f(a)=f(b)$, we then have $f(s(*))=f(t(*))$, so by [[Evaluations of Composite Functions]] $$f\circ s(*)=f\circ t(*).$$Since $*$ is the only member of $S$, based on this equality we can conclude that for all $x\in S$ we have $f\circ s(x)=f\circ t(x)$. Therefore, by [[Extensionality of Functions]] $f\circ s=f\circ t$. Since $f$ is a monomorphism, we must have $s=t$, so by [[Extensionality of Functions]] again $s(*)=t(*)$. We therefore have $a=b$. $\blacksquare$

**Proof of Backward Implication.** Suppose $f$ is injective. Suppose $X$ is a set, and suppose $s:X\to A$ and $t:X\to A$ satisfy $f\circ s=f\circ t$. Suppose $x\in X$. Then, by [[Extensionality of Functions]] $f\circ s(x)=f\circ t(x)$, so by [[Evaluations of Composite Functions]] $f(s(x))=f(t(x))$. Since $f$ is injective, we have $s(x)=t(x)$. By [[Extensionality of Functions]] again, this shows that $s=t$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Category of Sets]]
- [[Composition of Functions]]
- [[Injective Function]]
- [[Monomorphism]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]