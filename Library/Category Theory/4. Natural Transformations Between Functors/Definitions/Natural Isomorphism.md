**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$. A natural transformation $\nu:F\Rightarrow G$ is called a **natural isomorphism** if it satisfies any (and therefore, by [[Equivalence of Definitions of Natural Isomorphisms]], all) of the following properties.
1. $\nu$ is an isomorphism in $\mathsf{D}^\mathsf{C}$.
2. For all objects $a$ in $\mathsf{C}$, the morphism $\nu_{a}:F(a)\to G(a)$ is an isomorphism in $\mathsf{D}$.

Suppose $\nu:F\Rightarrow G$ is a natural isomorphism. Then, we say that $F$ and $G$ are **naturally isomorphic**. By definition, $\nu$ is then an isomorphism, so we can still write $$F\cong G.$$Moreover, for all objects $a$ in $\mathsf{C}$, we say that the isomorphism $\nu_{a}:F(a)\to G(a)$ is **natural** in $a$.
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Natural Transformation]]
- [[Functor Category]]

Theorems used:
- [[Equivalence of Definitions of Natural Isomorphisms]]