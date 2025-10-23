**Theorem.** Let $A$, $B$, and $C$ be sets. Let $f:A\to B$ and $g:B\to C$. Then, for all $a\in A$ we have $$g\circ f(a)=g(f(a)).$$
**Proof.** Suppose $a\in A$. For clarity, define $b\in C$ and $c\in C$ as objects such that $g\circ f(a)=b$ and $g(f(a))=c$. Then, we have $(a,b)\in g\circ f$. Also, $(f(a),c)\in g$ and $(a,f(a))\in f$, so $(a,c)\in g\circ f$. Since $g\circ f$ is a function, $b=c$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Composition of Functions]]