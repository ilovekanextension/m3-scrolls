**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. The **functor category** $\mathsf{D}^\mathsf{C}$ from $\mathsf{C}$ to $\mathsf{D}$
- has the following data:
	1. **Objects.** Objects in $\mathsf{D}^\mathsf{C}$ are functors $F:\mathsf{C}\to \mathsf{D}$.
	2. **Morphisms.** Morphisms in $\mathsf{D}^\mathsf{C}$ are natural transformations $\nu:F\Rightarrow G$.
- admits the following structure:
	1. **Identities.** Any functor $F:\mathsf{C}\to \mathsf{D}$ in $\mathsf{D}^\mathsf{C}$ has an identity natural transformation $\text{id}_{F}:F\Rightarrow F$.
	2. **Composition.** Natural transformations $\nu:F\Rightarrow G$ and $\sigma:G\Rightarrow H$ in $\mathsf{D}^\mathsf{C}$ can be composed into $\sigma\circ \nu:F\Rightarrow H$.

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Identity Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]