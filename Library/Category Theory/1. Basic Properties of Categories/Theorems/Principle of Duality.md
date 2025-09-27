**(Meta-)Theorem.** Let $\mathsf{C}$ be a category. Suppose $\Sigma$ is a categorical statement about $\mathsf{C}$. Then, the dual statement $\Sigma^\text{op}$ of $\Sigma$ obtained by reversing the direction of all morphisms i.e. replacing morphisms $f$ in $\Sigma$ with $f^\text{op}$ is a categorical statement about $\mathsf{C}^\text{op}$. Moreover, $\Sigma$ is true if and only if $\Sigma^\text{op}$ is true.

**Proof.** By definition,
- for all morphisms $f$ and $g$ in $\mathsf{C}$, if $f^\text{op}=g^\text{op}$, then $f=g$,
- for all objects $a$, $(\text{id}_{a})^\text{op}=\text{id}_{a}$, and
- for all morphisms $f:a\to b$ and $g:b\to c$, $(g\circ f)^\text{op}=f^\text{op}\circ g^\text{op}$.

Therefore, the truth of $\Sigma^\text{op}$ depends on the truth of $\Sigma$. Clearly $(\Sigma^\text{op})^\text{op}=\Sigma$, so the truth of $\Sigma$ also depends on the truth of $\Sigma ^\text{op}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Opposite Category]]