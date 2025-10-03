**Definition.** Let $\mathsf{C}$ be a locally small category. Let $F:\mathsf{C}\to \mathsf{Set}$. The **category of elements** $\int^{\mathsf{C}}F$ of $F$
- has the following data:
	1. **Objects.** Objects in $\int^{\mathsf{C}}F$ are pairs $(A,a)$, where $A$ is an object in $\mathsf{C}$ and $a\in F(A)$.
	2. **Morphisms.** A morphism $(A,a)\to(B,b)$ is a morphism $f:A\to B$ in $\mathsf{C}$ satisfying $[F(f)](a)=b$.
- admits the following structures:
	1. **Identities.** Any object $(A,a)$ in $\int^{\mathsf{C}}F$ has the identity morphism $\text{id}_{(A,a)}$.
	2. **Composition.** Compositions are inherited from $\mathsf{C}$.

Likewise, let $F:\mathsf{C}^\text{op}\to \mathsf{Set}$. The **category of elements** $\int_{\mathsf{C}}F$ of $F$
- has the following data:
	1. **Objects.** Objects in $\int_{\mathsf{C}}F$ are pairs $(A,a)$, where $A$ is an object in $\mathsf{C}$ and $a\in F(A)$.
	2. **Morphisms.** A morphism $(A,a)\to(B,b)$ is a morphism $f:A\to B$ in $\mathsf{C}$ satisfying $[F(f)](b)=a$.
- admits the following structures:
	1. **Identities.** Any object $(A,a)$ in $\int_{\mathsf{C}}F$ has the identity morphism $\text{id}_{(A,a)}$.
	2. **Composition.** Compositions are inherited from $\mathsf{C}$.

***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]