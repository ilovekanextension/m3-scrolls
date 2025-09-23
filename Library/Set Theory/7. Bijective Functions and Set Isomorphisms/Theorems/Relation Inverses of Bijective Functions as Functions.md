**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Then, $f$ is bijective if and only if $f^{-1}:B\to A$.

**Proof of Forward Implication.** Suppose $f$ is bijective.
- **Totality.** Suppose $b\in B$. Since $f$ is bijective, it is surjective, so there is $a\in A$ such that $(a,b)\in f$, which means $(b,a)\in f^{-1}$.
- **Functionality.** Suppose $b\in B$ and $x,y\in A$, and suppose that $(b,x)\in f^{-1}$ and $(b,y)\in f^{-1}$. Then, $(x,b)\in f$ and $(y,b)\in f$. Since $f$ is bijective, it is injective, so $x=y$. $\blacksquare$

**Proof of Backward Implication.** Suppose $f^{-1}:B\to A$.
- **Injectivity.** Suppose $a,b\in A$, and suppose that $f(a)=f(b)$. Define $c$ as the object in $B$ such that $f(a)=c$ and $f(b)=c$. We then have $(a,c)\in f$ and $(b,c)\in f$, so $(c,a)\in f^{-1}$ and $(c,b)\in f^{-1}$. Since $f^{-1}$ is a function, by functionality we therefore have $a=b$.
- **Surjectivity.** Suppose $b\in B$. Since $f^{-1}$ is a function, by totality there is $a\in A$ such that $(b,a)\in f^{-1}$ or $(a,b)\in f$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Inverse of Relation]]
- [[Function]]
- [[Injective Function]]
- [[Surjective Function]]
- [[Bijective Function]]