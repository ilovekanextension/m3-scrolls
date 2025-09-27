**Theorem.** Let $\mathsf{C}$ be a category. Then, the map $I$ on $\mathsf{C}$ that assigns
- to each object $A$ in $\mathsf{C}$ itself (so $I(A)=A$) and
- to each morphism $f:A\to B$ in $\mathsf{C}$ itself (so $I(f)=f$)

is a functor.

**Proof.**
- **Preservation of Identities.** Suppose $A$ is an object in $\mathsf{C}$. By definition of $I$, we have $$I(\text{id}_{A})=\text{id}_{A}=\text{id}_{I(A)}.$$
- **Preservation of Composition.** Suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. By definition of $I$, we have $$I(g\circ f)=g\circ f=I(g)\circ I(f). \blacksquare$$

***
Definitions used:
- [[Category]]
- [[Functor]]

