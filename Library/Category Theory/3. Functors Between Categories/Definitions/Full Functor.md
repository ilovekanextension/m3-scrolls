**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. We say that $F$ is **full** or **locally surjective** if for all objects $A$ and $B$ in $\mathsf{C}$, we have that for all morphisms $g:F(A)\to F(B)$ in $\mathsf{D}$, there is a morphism $f:A\to B$ in $\mathsf{C}$ such that $$F(f)=g.$$
This should not be confused with global surjectivity. Given a morphism $g:A'\to B'$ in $\mathsf{D}$, just because there already is a morphism $f:A\to B$ in $\mathsf{C}$ such that $F(f)=g$ doesn't mean there can be no other morphisms $h:C\to D$ in $\mathsf{C}$ not sharing identical source and target with $f$ such that $F(h)=g$, since we may have $F(C)=A'$ and $F(D)=B'$ (hence why we say "for all objects $A$ and $B$ in $\mathsf{C}$").
***
Definitions used:
- [[Category]]
- [[Functor]]