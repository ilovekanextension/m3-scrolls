**Theorem.** Let $A$, $B$, and $C$ be sets. Let $f:A\to B$ and $g:B\to C$. Then, $g\circ f:A\to C$.

**Proof.**
- **Totality.** Suppose $a\in A$. Since $f$ is a function, there is $b\in B$ such that $(a,b)\in f$. Since $g$ is also a function, there is $c\in C$ such that $(b,c)\in g$. Therefore, $(a,c)\in g\circ f$.
- **Functionality.** Suppose $a\in A$ and $b,c\in C$, and suppose that $(a,b)\in g\circ f$ and $(a,c)\in g\circ f$. Then, there are objects $x,y\in B$ such that $(a,x)\in f$, $(x,b)\in g$, $(a,y)\in f$, and $(y,c)\in g$. Since $f$ is a function, we have $x=y$. This means $(x,b)\in g$ and $(x,c)\in g$. Since $g$ is a function, $b=c$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Composition of Relations]]
- [[Function]]