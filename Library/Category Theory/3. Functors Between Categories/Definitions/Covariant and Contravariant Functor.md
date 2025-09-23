**Definition.** A functor $F:\mathsf{C}\to \mathsf{D}$ is said to be **covariant** from $\mathsf{C}$ to $\mathsf{D}$, and a functor $$G:\mathsf{C}^\text{op}\to \mathsf{D}$$is said to be **contravariant** from $\mathsf{C}$ to $\mathsf{D}$ (notice the categories mentioned; we can still say that $G$ is covariant from $\mathsf{C}^\text{op}$ to $\mathsf{D}$). A contravariant functor from $\mathsf{C}$ to $\mathsf{D}$ is best viewed as a map from $\mathsf{C}$, instead of $\mathsf{C}^\text{op}$, to $\mathsf{D}$ by pre-composing a covariant functor $\mathsf{C}^\text{op}\to \mathsf{D}$ with the map $$(-)^\text{op}:f\mapsto f^\text{op}$$from $\mathsf{C}$ to $\mathsf{C}^\text{op}$.

Therefore, a contravariant functor from $\mathsf{C}$ to $\mathsf{D}$ may also be defined as a map $F$ that assigns
- to each object $a$ in $\mathsf{C}$ an object $F(a)$ in $\mathsf{D}$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ a morphism $F(f):F(b)\to F(a)$ in $\mathsf{D}$

satisfying the following properties.
- **Preservation of Identities.** For all objects $a$ in $\mathsf{C}$, $$F(\text{id}_{a})=\text{id}_{F(a)}.$$
- **Preservation of Composition.** For all morphisms $f:a\to b$ and $g:b\to c$ in $\mathsf{C}$, $$F(g\circ f)=F(f)\circ F(g).$$

***
Definitions used:
- [[Category]]
- [[Opposite Category]]
- [[Functor]]