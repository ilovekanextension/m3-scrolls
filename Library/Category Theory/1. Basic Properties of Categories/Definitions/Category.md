**Definition.** A **category** $\mathsf{C}$ is a mathematical structure that
- has the following data:
	  1. **Objects.** The collection of all objects in $\mathsf{C}$ is denoted as $\text{Ob}(\mathsf{C})$.
	  2. **Morphism.** The collection of all morphisms in $\mathsf{C}$ is denoted as $\text{Hom}(\mathsf{C})$. The collection of all morphisms from $a$ to $b$ in $\mathsf{C}$ is denoted $\mathsf{C}(a,b)$.
- admits the following structures:
	  1. **Identities.** Any object $a$ in $\mathsf{C}$ has an identity morphism $\text{id}_{a}:a\to a$.
	  2. **Composition.** Morphisms $f:a\to b$ and $g:b\to c$ may be composed into $g\circ f:a\to b$.
- follows the following properties:
	  1. **Associativity Law.** For all morphisms $f:a\to b$, $g:b\to c$, and $h:c\to d$, we have $$(h\circ g)\circ f=h\circ(g\circ f).$$
	  2. **Unit Law.** For all morphisms $f:a\to b$, we have $$f\circ \text{id}_{a}=f=\text{id}_{b}\circ f.$$
