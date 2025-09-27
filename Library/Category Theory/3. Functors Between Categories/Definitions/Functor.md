**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. A map $F$ from $\mathsf{C}$ to $\mathsf{D}$ that assigns
- to each object $A$ in $\mathsf{C}$ an object $F(A)$ in $\mathsf{D}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ a morphism $F(f):F(A)\to F(B)$ in $\mathsf{D}$

is called a **functor** if it satisfies the following properties.
1. **Preservation of Identities.** For all objects $A$ in $\mathsf{C}$, we have $$F(\text{id}_{A})=\text{id}_{F(A)}.$$
2. **Preservation of Composition.** For all morphisms $f:A\to B$ and $g:B\to C$ in $\mathsf{C}$, we have $$F(g\circ f)=F(g)\circ F(f).$$

If $F$ is a functor from $\mathsf{C}$ to $\mathsf{D}$, we may write $$F:\mathsf{C}\to \mathsf{D}.$$
***
Definitions used:
- [[Category]]