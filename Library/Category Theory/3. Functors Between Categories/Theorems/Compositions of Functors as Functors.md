**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{E}$. Then, the map $H$ from $\mathsf{C}$ to $\mathsf{E}$ that assigns
- to each object $a$ in $\mathsf{C}$ the object $H(a)=G(F(a))$ in $\mathsf{E}$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ the morphism $H(f)=G(F(f))$ in $\mathsf{E}$

is a functor.

**Proof.**
- **Preservation of Identities.** Suppose $a$ is an object in $\mathsf{C}$. Since $F$ is a functor, by definition it preserves identity morphisms, so $$F(\text{id}_{a})=\text{id}_{F(a)}.$$Since $G$ is a functor, by definition it also preserves identity morphisms, so $$G(\text{id}_{F(a)})=\text{id}_{G(F(a))}.$$We therefore have 
  $$\begin{align}
H(\text{id}_{a}) & =G(F(\text{id}_{a})) \\
 & =G(\text{id}_{F(a)}) \\
 & =\text{id}_{G(F(a))} \\
 & =\text{id}_{H(a)}.
\end{align}$$
- **Preservation of Composition.** Suppose $f:a\to b$ and $g:b\to c$ are morphisms in $\mathsf{C}$. Since $F$ is a functor, by definition it preserves composition, so $$F(g\circ f)=F(g)\circ F(f).$$Since $G$ is a functor, by definition it also preserves composition, so $$G(F(g)\circ F(f))=G(F(g))\circ G(F(f)).$$We therefore have
  $$\begin{align}
H(g\circ f) & =G(F(g\circ f)) \\
 & =G(F(g)\circ F(f)) \\
 & =G(F(g))\circ G(F(f)) \\
 & =H(g)\circ H(f). \blacksquare
\end{align}$$


***
Definitions used:
- [[Category]]
- [[Functor]]
