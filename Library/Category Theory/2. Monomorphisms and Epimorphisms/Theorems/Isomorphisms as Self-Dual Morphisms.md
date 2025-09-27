**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be an isomorphism in $\mathsf{C}$. Then, $f^\text{op}:B\to A$ is also an isomorphism in $\mathsf{C}^\text{op}$ and $$(f^\text{op})^{-1}=(f^{-1})^\text{op}.$$Hence, we say that isomorphisms are **self-dual**.

**Proof.** Since $f$ is an isomorphism, we have $f^{-1}\circ f=\text{id}_{A}$ and $f\circ f^{-1}=\text{id}_{B}$. Therefore, by definition of duals we have $$f^\text{op}\circ (f^{-1})^\text{op}=(f^{-1}\circ f)^\text{op}=(\text{id}_{A})^\text{op}=\text{id}_{A}$$and $$(f^{-1})^\text{op}\circ f^\text{op}=(f\circ f^{-1})^\text{op}=(\text{id}_{B})^\text{op}=\text{id}_{B},$$so $f^\text{op}$ is an isomorphism with inverse $(f^{-1})^\text{op}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Opposite Category]]
 