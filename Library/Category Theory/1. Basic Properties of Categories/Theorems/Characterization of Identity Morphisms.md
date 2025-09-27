**Theorem.** Let $\mathsf{C}$ be a category. Let $i:A\to A$ be a morphism in $\mathsf{C}$.
1. Suppose that for all morphisms $f:A\to B$ we have $$f\circ i=f.$$Then, $i=\text{id}_{A}$.
2. Suppose that for all morphisms $g:B\to A$ we have $$i\circ g=g.$$Then, $i=\text{id}_{A}$.

**Proof of First Statement.** By assumption, $\text{id}_{A}\circ i=\text{id}_{A}$. By the unit law, $\text{id}_{A}\circ i=i$. Therefore, $i=\text{id}_{A}$. $\blacksquare$

**Proof of Second Statement.** By assumption, $i\circ \text{id}_{A}=\text{id}_{A}$. By the unit law, $i\circ \text{id}_{A}=i$. Therefore, $i=\text{id}_{A}$. $\blacksquare$
***
Definitions used:
- [[Category]]