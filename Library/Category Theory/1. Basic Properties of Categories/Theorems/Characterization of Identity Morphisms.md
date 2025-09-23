**Theorem.** Let $\mathsf{C}$ be a category. Let $i:a\to a$ be a morphism in $\mathsf{C}$.
1. Suppose that for all morphisms $f:a\to b$ we have $$f\circ i=f.$$Then, $i=\text{id}_{a}$.
2. Suppose that for all morphisms $g:b\to a$ we have $$i\circ g=g.$$Then, $i=\text{id}_{a}$.

**Proof of First Statement.** By assumption, $\text{id}_{a}\circ i=\text{id}_{a}$. By the unit law, $\text{id}_{a}\circ i=i$. Therefore, $i=\text{id}_{a}$. $\blacksquare$

**Proof of Second Statement.** By assumption, $i\circ \text{id}_{a}=\text{id}_{a}$. By the unit law, $i\circ \text{id}_{a}=i$. Therefore, $i=\text{id}_{a}$. $\blacksquare$
***
Definitions used:
- [[Category]]