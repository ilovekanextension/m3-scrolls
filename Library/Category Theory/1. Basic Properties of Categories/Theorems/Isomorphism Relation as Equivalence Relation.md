**Theorem.** Let $\mathsf{C}$ be a category.
1. For all objects $a$ in $\mathsf{C}$, $a\cong a$.
2. For all objects $a$ and $b$ in $\mathsf{C}$, if $a\cong b$, then $b\cong a$.
3. For all objects $a$, $b$, and $c$ in $\mathsf{C}$, if $a\cong b$ and $b\cong c$, then $a\cong c$.

**Proof of First Statement.** Suppose $a$ is an object in $\mathsf{C}$. By [[Identity Morphisms as Isomorphisms]], $\text{id}_{a}:a\to a$ is an isomorphism, so $a\cong a$. $\blacksquare$

**Proof of Second Statement.** Suppose $a$ and $b$ are objects in $\mathsf{C}$. Suppose $a\cong b$. Then, there is an isomorphism $f:a\to b$. By [[Inverses of Isomorphisms as Isomorphisms]], $f^{-1}:b\to a$ is also an isomorphism, so $b\cong a$. $\blacksquare$

**Proof of Third Statement.** Suppose $a$, $b$, and $c$ are objects in $\mathsf{C}$. Suppose $a\cong b$ and $b\cong c$. Then, there are isomorphisms $f:a\to b$ and $g:b\to c$. By [[Compositions of Isomorphisms as Isomorphisms]], $g\circ f:a\to c$ is also an isomorphism, so $a\cong c$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]

Theorems used:
- [[Identity Morphisms as Isomorphisms]]
- [[Inverses of Isomorphisms as Isomorphisms]]
- [[Compositions of Isomorphisms as Isomorphisms]]