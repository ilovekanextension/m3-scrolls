Let $\mathsf{C}$ be a category. An object $t$ in $\mathsf{C}$ is said to be **terminal** if for all objects $a$ in $\mathsf{C}$ there is a unique morphism $f:a\to t$.

**Theorem.** Let $\mathsf{C}$ be a category. Suppose $s$ and $t$ are both terminal objects in $\mathsf{C}$. Then, $s\cong t$. Hence, terminal objects are unique up to isomorphism.

In fact, the isomorphism $s\cong t$ is unique, so terminal objects are actually unique up to a **unique** isomorphism.

**Proof.** Since $s$ is terminal and $t$ is in $\mathsf{C}$, there is a morphism $f: t\to s$. Likewise, since $t$ is terminal and $s$ is in $\mathsf{C}$, there is a morphism $g:s\to t$. We then have $g\circ f: t\to t$ and $f\circ g:s\to s$. Since $t$ is terminal, the morphism $t\to t$ must be unique. We have $g\circ f: t\to t$ and $\text{id}_{t}: t\to t$, so $g\circ f=\text{id}_{t}$. By the same reasoning, $f\circ g=\text{id}_{s}$. This means $f$ is an isomorphism with inverse $g$, so $s\cong t$.

Now suppose $f:s\to t$ and $g:s\to t$ are both isomorphisms. Since $t$ is terminal, we must have $f=g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]