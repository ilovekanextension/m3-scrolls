**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $x$ be an object in $\mathsf{D}$. Then, the map $F$ from $\mathsf{C}$ to $\mathsf{D}$ that assigns
- to each object $a$ in $\mathsf{C}$ the object $x$ and
- to each morphism $f:a\to b$ the morphism $\text{id}_{x}:x\to x$

is a functor.

**Proof.**
- **Preservation of Identities.** Suppose $a$ is an object in $\mathsf{C}$. By definition, $$F(\text{id}_{a})=\text{id}_{x}=\text{id}_{F(a)}.$$
- **Preservation of Composition.** Suppose $f:a\to b$ and $g:b\to c$ are morphisms in $\mathsf{C}$. By definition, $$F(g\circ f)=\text{id}_{x}=\text{id}_{x}\circ\text{id}_{x}=F(g)\circ F(f).\blacksquare$$

***
Definitions used:
- [[Category]]
- [[Functor]]