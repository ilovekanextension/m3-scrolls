**Definition.** A **category** $\mathsf{C}$ is a mathematical structure that
- has the following data:
	  1. **Objects.** The collection of all objects in $\mathsf{C}$ is denoted as $\text{Ob}(\mathsf{C})$.
	  2. **Morphism.** The collection of all morphisms in $\mathsf{C}$ is denoted as $\text{Hom}(\mathsf{C})$. Given objects $A$ and $B$ of $\mathsf{C}$, the collection of all morphisms from $A$ to $B$ in $\mathsf{C}$ is denoted $\mathsf{C}(A,B)$.
- admits the following structures:
	  1. **Identities.** Any object $A$ in $\mathsf{C}$ has an identity morphism $\text{id}_{A}:A\to A$.
	  2. **Composition.** Morphisms $f:A\to B$ and $g:B\to C$ may be composed into $g\circ f:A\to C$.
- follows the following properties:
	  1. **Associativity Law.** For all morphisms $f:A\to B$, $g:B\to C$, and $h:C\to D$, we have $$(h\circ g)\circ f=h\circ(g\circ f).$$
	  2. **Unit Law.** For all morphisms $f:A\to B$, we have $$f\circ \text{id}_{A}=\text{id}_{B}\circ f=f.$$
