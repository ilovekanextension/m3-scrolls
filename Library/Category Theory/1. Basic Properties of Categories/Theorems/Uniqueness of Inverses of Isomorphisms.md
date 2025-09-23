Let $\mathsf{C}$ be a category. Let $f:a\to b$ be a morphism in $\mathsf{C}$. An **inverse** of $f$ is a morphism $g:b\to a$ in $\mathsf{C}$ satisfying $g\circ f=\text{id}_{a}$ and $f\circ g=\text{id}_{b}$.

**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ be a morphism in $\mathsf{C}$. Suppose $g:b\to a$ and $h:b\to a$ are both inverses of $f$. Then, $g=h$.

**Proof.** Since $g$ is an inverse of $f$, we have $f\circ g=\text{id}_{b}$. Since $h$ is an inverse of $f$, we have $h\circ f=\text{id}_{a}$. Therefore, $$g=\text{id}_{a}\circ g=(h\circ f)\circ g=h\circ(f\circ g)=h\circ \text{id}_{b}=h. \blacksquare$$
***
Definitions used:
- [[Category]]