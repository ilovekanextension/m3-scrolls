**Theorem.** Let $\mathsf{I}$ and $\mathsf{C}$ be categories, and suppose that $\mathsf{I}$ is small. Let $F:\mathsf{I}\to \mathsf{C}$. Then, the map that assigns
- to each object $A$ in $\mathsf{C}^\text{op}$ the set $\text{Cone}(A,F)$ in $\mathsf{Set}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}^\text{op}$ the function $\text{Cone}(B,F)\to \text{Cone}(A,F)$ that maps a cone $(B,\sigma)$ to the cone $(A,\nu)$, where $\nu$ is the natural transformation (well-defined by [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]) defined as $$\nu_{X}=\sigma_{X}\circ f$$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}$. Likewise, the map $H$ that assigns
- to each object $A$ in $\mathsf{C}$ the set $\text{Cone}(F,A)$ in $\mathsf{Set}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ the function $\text{Cone}(F,A)\to \text{Cone}(F,B)$ that maps a cone $(A,\sigma)$ to the cone $(B,\nu)$, where $\nu$ is the natural transformation (well-defined by [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]) defined as $$\nu_{X}=f\circ\sigma_{X}$$

is a functor from $\mathsf{C}$ to $\mathsf{Set}$.

**Proof of First Statement.** 