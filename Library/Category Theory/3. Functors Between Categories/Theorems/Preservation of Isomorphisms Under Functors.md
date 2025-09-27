**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. Suppose $f:A\to B$ is an isomorphism in $\mathsf{C}$. Then, $F(f):F(A)\to F(B)$ is an isomorphism in $\mathsf{D}$ and $$F(f)^{-1}=F(f^{-1}).$$
**Proof.** Since $f$ is an isomorphism, we have $f^{-1}\circ f=\text{id}_{A}$ and $f\circ f^{-1}=\text{id}_{B}$. Since $F$ is a functor, we have $$F(f^{-1})\circ F(f)=F(f^{-1}\circ f)=F(\text{id}_{A})=\text{id}_{F(A)}$$and $$F(f)\circ F(f^{-1})=F(f\circ f^{-1})=F(\text{id}_{B})=\text{id}_{F(B)}.$$Therefore, $F(f)$ is an isomorphism with inverse $F(f^{-1})$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]