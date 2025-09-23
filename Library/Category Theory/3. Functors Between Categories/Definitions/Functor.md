**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. A map $F$ from $\mathsf{C}$ to $\mathsf{D}$ that assigns
- to each object $a$ in $\mathsf{C}$ an object $F(a)$ in $\mathsf{D}$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ a morphism $F(f):F(a)\to F(b)$ in $\mathsf{D}$

is called a **functor** if it satisfies the following properties.
1. **Preservation of Identities.** For all objects $a$ in $\mathsf{C}$, we have $$F(\text{id}_{a})=\text{id}_{F(a)}.$$
2. **Preservation of Composition.** For all morphisms $f:a\to b$ and $g:b\to c$ in $\mathsf{C}$, we have $$F(g\circ f)=F(g)\circ F(f).$$

***
Definitions used:
- [[Category]]