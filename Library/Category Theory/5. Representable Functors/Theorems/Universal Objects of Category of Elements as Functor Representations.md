**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $F:\mathsf{C}\to \mathsf{Set}$. Suppose $(X,u)$ is a pair in $\int^\mathsf{C}F$. Then, $\gamma(u):h^X\Rightarrow F$ (see [[Yoneda Lemma]] for definition of $\gamma$) is a natural isomorphism if and only if for all pairs $(A,a)$ in $\int^\mathsf{C}F$ there is a unique morphism $f:(X,u)\to(A,a)$.

Likewise, let $F:\mathsf{C}^\text{op}\to \mathsf{Set}$. Suppose $(X,u)$ is a pair in $\int_\mathsf{C}F$. Then, $\gamma(u):h_{X}\Rightarrow F$ is a natural isomorphism if and only if for all pairs $(A,a)$ in $\int_\mathsf{C}F$ there is a unique morphism $f:(A,a)\to(X,u)$.

**Proof of First Statement.** First suppose $\gamma(u)$ is a natural isomorphism. Suppose $(A,a)$ is a pair in $\int^\mathsf{C}F$. Since $\gamma(u)$ is a natural isomorphism, for all objects $Y$ in $\mathsf{C}$ the function $\gamma(u)_{Y}$ is an isomorphism. In particular, since $A$ is an object in $\mathsf{C}$, $\gamma(u)_{A}$ is an isomorphism. By [[Bijective Functions as Isomorphisms]], $\gamma(u)_{A}$ is then a bijection. Since $a\in F(A)$, this means there is a unique morphism $f:X\to A$ such that $[\gamma(u)_{A}](f)=a$ or, by definition of $\gamma$, $[F(f)](u)=a$. This is precisely the condition of $f$ being a morphism from $(X,u)$ to $(A,a)$.

Now suppose that for all pairs $(A,a)$ in $\int^\mathsf{C}F$ there is a unique morphism $f:(X,u)\to(A,a)$. To prove that $\gamma(u)$ is a natural isomorphism, we need to show that for all objects $A$ in $\mathsf{C}$ the function $\gamma(u)_{A}:\mathsf{C}(X,A)\to F(A)$ is an isomorphism. By [[Bijective Functions as Isomorphisms]] it is enough to show that $\gamma(u)_{A}$ is a bijection, which is to show that for all $a\in F(A)$ there is a unique morphism $f:X\to A$ such that $[\gamma(u)_{A}](f)=a$ or $[F(f)](u)=a$. This is precisely the content of the given assumption. $\blacksquare$

**Proof of Second Statement.** First suppose $\gamma(u)$ is a natural isomorphism. Suppose $(A,a)$ is a pair in $\int_\mathsf{C}F$. Since $\gamma(u)$ is a natural isomorphism, for all objects $Y$ in $\mathsf{C}$ the function $\gamma(u)_{Y}$ is an isomorphism. In particular, since $A$ is an object in $\mathsf{C}$, $\gamma(u)_{A}$ is an isomorphism. By [[Bijective Functions as Isomorphisms]], $\gamma(u)_{A}$ is then a bijection. Since $a\in F(A)$, this means there is a unique morphism $f:A\to X$ such that $[\gamma(u)_{A}](f)=a$ or, by definition of $\gamma$, $[F(f)](u)=a$. This is precisely the condition of $f$ being a morphism from $(A,a)$ to $(X,u)$.

Now suppose that for all pairs $(A,a)$ in $\int_\mathsf{C}F$ there is a unique morphism $f:(A,a)\to(X,u)$. To prove that $\gamma(u)$ is a natural isomorphism, we need to show that for all objects $A$ in $\mathsf{C}$ the function $\gamma(u)_{A}:\mathsf{C}(A,X)\to F(A)$ is an isomorphism. By [[Bijective Functions as Isomorphisms]] it is enough to show that $\gamma(u)_{A}$ is a bijection, which is to show that for all $a\in F(A)$ there is a unique morphism $f:A\to X$ such that $[\gamma(u)_{A}](f)=a$ or $[F(f)](u)=a$. This is precisely the content of the given assumption. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Natural Transformation]]
- [[Natural Isomorphism]]
- [[Hom-Functor]]
- [[Category of Elements]]
- [[Bijective Function]]

Theorems used:
- [[Yoneda Lemma]]
- [[Bijective Functions as Isomorphisms]]