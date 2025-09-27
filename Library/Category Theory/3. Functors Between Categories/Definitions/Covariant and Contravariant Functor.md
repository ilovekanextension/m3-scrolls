**Definition.** A functor $F:\mathsf{C}\to \mathsf{D}$ is said to be **covariant** from $\mathsf{C}$ to $\mathsf{D}$, and a functor $$G:\mathsf{C}^\text{op}\to \mathsf{D}$$is said to be **contravariant** from $\mathsf{C}$ to $\mathsf{D}$. A contravariant functor from $\mathsf{C}$ to $\mathsf{D}$ is best viewed as a map from $\mathsf{C}$ to $\mathsf{D}$ obtained by pre-composing a covariant functor $\mathsf{C}^\text{op}\to \mathsf{D}$ with the map $$(-)^\text{op}:f\mapsto f^\text{op}$$from $\mathsf{C}$ to $\mathsf{C}^\text{op}$.

Therefore, a contravariant functor from $\mathsf{C}$ to $\mathsf{D}$ may also be defined as a map $F$ that assigns
- to each object $A$ in $\mathsf{C}$ an object $F(a)$ in $\mathsf{D}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ a morphism $F(f):F(b)\to F(a)$ in $\mathsf{D}$

satisfying the following properties.
- **Preservation of Identities.** For all objects $A$ in $\mathsf{C}$, $$F(\text{id}_{A})=\text{id}_{F(A)}.$$
- **Preservation of Composition.** For all morphisms $f:A\to B$ and $g:B\to C$ in $\mathsf{C}$, $$F(g\circ f)=F(f)\circ F(g).$$

***
Definitions used:
- [[Category]]
- [[Opposite Category]]
- [[Functor]]