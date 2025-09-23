**Theorem.** Let $\mathsf{C}$ be a category. Then, the map $I$ on $\mathsf{C}$ that assigns
- to each object $a$ in $\mathsf{C}$ itself (so $I(a)=a$) and
- to each morphism $f:a\to b$ in $\mathsf{C}$ itself (so $I(f)=f$)

is a functor.

**Proof.**
- **Preservation of Identities.** Suppose $a$ is an object in $\mathsf{C}$. By definition of $I$, we have $$I(\text{id}_{a})=\text{id}_{a}=\text{id}_{I(a)}.$$
- **Preservation of Composition.** Suppose $f:a\to b$ and $g:b\to c$ are morphisms in $\mathsf{C}$. By definition of $I$, we have $$I(g\circ f)=g\circ f=I(g)\circ I(f). \blacksquare$$

***
Definitions used:
- [[Category]]
- [[Functor]]

