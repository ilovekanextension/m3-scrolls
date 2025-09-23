**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F$ be a functor from $\mathsf{C}$ to $\mathsf{D}$. Suppose $f:a\to b$ is an isomorphism in $\mathsf{C}$. Then, $F(f):F(a)\to F(b)$ is an isomorphism in $\mathsf{D}$ and $$F(f)^{-1}=F(f^{-1}).$$
**Proof.** Since $f$ is an isomorphism, we have $f^{-1}\circ f=\text{id}_{a}$ and $f\circ f^{-1}=\text{id}_{b}$. Since $F$ is a functor, we have $$F(f^{-1})\circ F(f)=F(f^{-1}\circ f)=F(\text{id}_{a})=\text{id}_{F(a)}$$and $$F(f)\circ F(f^{-1})=F(f\circ f^{-1})=F(\text{id}_{b})=\text{id}_{F(b)}.$$Therefore, $F(f)$ is an isomorphism with inverse $F(f^{-1})$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]