**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ be an isomorphism in $\mathsf{C}$. Then, $f^\text{op}:b\to a$ is also an isomorphism in $\mathsf{C}^\text{op}$ and $$(f^\text{op})^{-1}=(f^{-1})^\text{op}.$$Hence, we say that isomorphism is a **self-dual** concept.

**Proof.** Since $f$ is an isomorphism, we have $f^{-1}\circ f=\text{id}_{a}$ and $f\circ f^{-1}=\text{id}_{b}$. Therefore, by definition of duals we have $$f^\text{op}\circ (f^{-1})^\text{op}=(f^{-1}\circ f)^\text{op}=(\text{id}_{a})^\text{op}=\text{id}_{a}$$and $$(f^{-1})^\text{op}\circ f^\text{op}=(f\circ f^{-1})^\text{op}=(\text{id}_{b})^\text{op}=\text{id}_{b},$$so $f^\text{op}$ is an isomorphism with inverse $(f^{-1})^\text{op}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Opposite Category]]
 