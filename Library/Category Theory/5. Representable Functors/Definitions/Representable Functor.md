**Definition.** Let $\mathsf{C}$ be a locally small category. Let $F:\mathsf{C}\to\mathsf{Set}$. A **representation** $(X,\nu)$ of $F$ consists of
- an object $X$ in $\mathsf{C}$ and
- a natural isomorphism $\nu:h^X\Rightarrow F$.

Likewise, let $F:\mathsf{C}^\text{op}\to\mathsf{Set}$. A **representation** $(X,\nu)$ of $F$ consists of
- an object $X$ in $\mathsf{C}$ and
- a natural isomorphism $\nu:h_{X}\Rightarrow F$.

Equivalently, by [[Universal Objects of Category of Elements as Functor Representations]], a representation $(X,u)$ of $F:\mathsf{C}\to \mathsf{Set}$ (respectively $F:\mathsf{C}^\text{op}\to \mathsf{Set}$) consists of
- an object $X$ in $\mathsf{C}$ and
- an element $u\in F(X)$, called a **universal element** of $F$

satisfying the following property: for all objects $A$ in $\mathsf{C}$ and elements $a\in F(A)$, there is a unique morphism $f:X\to A$ (respectively $f:A\to X$) such that $[F(f)](u)=a$.

A representation of $F$ is therefore essentially a presentation of $F$ as a hom-functor. In both cases, we say that $F$ is **representable** and that $X$ **represents** $F$ (or $F$ is **represented** by $X$). When using $(X,u)$ as a representation of $F$, we say that $X$ together with $u$ has a **universal property**.
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Natural Isomorphism]]
- [[Hom-Functor]]
- [[Category of Sets]]

Theorems used:
- [[Universal Objects of Category of Elements as Functor Representations]]