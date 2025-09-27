**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $X$ be an object in $\mathsf{D}$. Then, the map $F$ from $\mathsf{C}$ to $\mathsf{D}$ that assigns
- to each object $A$ in $\mathsf{C}$ the object $X$ and
- to each morphism $f:A\to B$ the morphism $\text{id}_{X}:X\to X$

is a functor.

**Proof.**
- **Preservation of Identities.** Suppose $A$ is an object in $\mathsf{C}$. By definition, $$F(\text{id}_{A})=\text{id}_{X}=\text{id}_{F(A)}.$$
- **Preservation of Composition.** Suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. By definition, $$F(g\circ f)=\text{id}_{X}=\text{id}_{X}\circ\text{id}_{X}=F(g)\circ F(f).\blacksquare$$

***
Definitions used:
- [[Category]]
- [[Functor]]