**Definition.** Let $\mathsf{C}$ be a category. The **opposite category** of $\mathsf{C}$, denoted $\mathsf{C}^\text{op}$
- has the following data:
	1. **Objects.** Objects in $\mathsf{C}^\text{op}$ are the same as objects in $\mathsf{C}$.
	2. **Morphisms.** Morphisms in $\mathsf{C}^\text{op}$ are the same as morphisms in $\mathsf{C}$ except with reversed direction. A morphism in $\mathsf{C}^\text{op}$ will always be identified by its corresponding morphism in $\mathsf{C}$ with an "$\text{op}$" superscript. For example, $f^\text{op}:b\to a$ is meant to be understood as the morphism $f:a\to b$ in $\mathsf{C}$.
- admits the following structures:
	1. **Identities.** Identity morphisms in $\mathsf{C}^\text{op}$ are the same as identity morphisms in $\mathsf{C}$.
	2. **Composition.** Composition in $\mathsf{C}^\text{op}$ is inherited from $\mathsf{C}$.

By the definitions given, we have the following properties.
- For all morphisms $f:a\to b$ and $g:a\to b$ in $\mathsf{C}$, if $f^\text{op}=g^\text{op}$, then $f=g$.
- For all objects $a$ in $\mathsf{C}$, $\text{id}_{a}^\text{op}=\text{id}_{a}$.
- For all morphisms $f:a\to b$ and $g:b\to c$ in $\mathsf{C}$, $(g\circ f)^\text{op}=f^\text{op}\circ g^\text{op}$.

The morphism $f^\text{op}$ is usually called the **dual** of $f$.
***
Definitions used:
- [[Category]]