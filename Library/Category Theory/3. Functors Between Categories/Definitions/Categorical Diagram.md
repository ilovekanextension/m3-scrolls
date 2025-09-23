**Definition.** Let $\mathsf{C}$ be a category. A **diagram** of $\mathsf{C}$ is a collection of objects and morphisms in $\mathsf{C}$ that is closed under composition and identities. That is,
- if $a$ is an object in the diagram, then $\text{id}_{a}$ is also in the diagram, and
- if $f:a\to b$ and $g:b\to c$ are morphisms in the diagram, then $g\circ f:a\to c$ is also in the diagram.

Technically, a diagram of $\mathsf{C}$ is therefore just (the image of) a functor $F$ from a category $\mathsf{I}$ to $\mathsf{C}$. We proceed to say that $\mathsf{I}$ is the **index** of $F$ and that $F$ has the **shape** of $\mathsf{I}$.

We say that a diagram **commutes** or **is commutative** if for all morphisms $f$ and $g$ in the diagram sharing the same source and target, we have $f=g$.
***
Definitions used:
- [[Category]]
- [[Functor]]