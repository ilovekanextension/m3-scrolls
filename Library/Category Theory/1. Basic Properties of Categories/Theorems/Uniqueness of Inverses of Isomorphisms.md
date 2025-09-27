Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a morphism in $\mathsf{C}$. An **inverse** of $f$ is a morphism $g:B\to A$ in $\mathsf{C}$ satisfying $g\circ f=\text{id}_{A}$ and $f\circ g=\text{id}_{B}$.

**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a morphism in $\mathsf{C}$. Suppose $g:B\to A$ and $h:B\to A$ are both inverses of $f$. Then, $g=h$.

**Proof.** Since $g$ is an inverse of $f$, we have $f\circ g=\text{id}_{B}$. Since $h$ is an inverse of $f$, we have $h\circ f=\text{id}_{A}$. Therefore, $$g=\text{id}_{A}\circ g=(h\circ f)\circ g=h\circ(f\circ g)=h\circ \text{id}_{B}=h. \blacksquare$$
***
Definitions used:
- [[Category]]