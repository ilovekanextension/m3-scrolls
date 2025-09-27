**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. We say that $F$ is **faithful** or **locally injective** if for all objects $A$ and $B$ in $\mathsf{C}$, we have that for all morphisms $f:A\to B$ and $g:A\to B$ satisfying $$F(f)=F(g)$$we have $f=g$.

This should not be confused with global injectivity. Two morphisms $f:A\to B$ and $g:C\to D$ in $\mathsf{C}$ with $F(f)=F(g)$ need not be the same when $f$ does not necessarily share identical source and target with $g$ (hence why we say "for all objects $A$ and $B$ in $\mathsf{C}$").
***
Definitions used:
- [[Category]]
- [[Functor]]