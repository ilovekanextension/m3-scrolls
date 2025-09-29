**Theorem.** Let $\mathsf{C}$ be a locally small category. Then, the Yoneda embeddings $h^{\bullet}:\mathsf{C}^\text{op}\to \mathsf{Set}^\mathsf{C}$ and $h_{\bullet}:\mathsf{C}\to \mathsf{Set}^{\mathsf{C}^\text{op}}$ are full and faithful.

**Proof of First Statement.** Suppose $A$ and $B$ are objects in $\mathsf{C}$. By [[Yoneda Lemma]], the functions $\phi:\mathsf{Set}^\mathsf{C}(h^A,h^B)\to h^B(A)$ and $\gamma:h^B(A)\to \mathsf{Set}^\mathsf{C}(h^A,h^B)$ defined as $$\phi(\alpha)=\alpha_{A}(\text{id}_{A})\wedge \gamma(f)=\{s_{A\to X}\mapsto[h^B(s)](f)\}_{X\in \text{Ob}(\mathsf{C})}$$are isomorphisms and inverses of each other. We will first show that for all morphisms $f:B\to A$, $\gamma(f)=h^f$.

Suppose $X$ is an object in $\mathsf{C}$. Suppose $s:A\to X$ is a morphism in $\mathsf{C}$. We have
$$\begin{align}
[\gamma(f)_{X}](s) & =[h^B(s)](f) \\
 & =s\circ f \\
 & =(h^f)_{X}(s).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $\gamma(f)=h^f$.

We now show that for all natural transformations $\alpha:h^A\Rightarrow h^B$ there is a unique morphism $f:B\to A$ such that $h^f=\alpha$; this then proves that $h^\bullet$ is full and faithful.
Suppose $\alpha:h^A\Rightarrow h^B$.
- **Existence.** We pick $f=\phi(\alpha)$. Since $\phi$ and $\gamma$ are inverses, $$h^f=\gamma(f)=\gamma(\phi(\alpha))=\alpha.$$
- **Uniqueness.** Suppose $f:B\to A$ and $g:B\to A$ satisfy $h^f=\alpha$ and $h^g=\alpha$. Then, $h^f=h^g$, so $\gamma(f)=\gamma(g)$. This means $$\phi(\gamma(f))=\phi(\gamma(g)),$$so, since $\phi$ and $\gamma$ are inverses, $f=g$. $\blacksquare$

**Proof of Second Statement.** Suppose $A$ and $B$ are objects in $\mathsf{C}$. By [[Yoneda Lemma]], the functions $\phi:\mathsf{Set}^\mathsf{C}(h_{A},h_{B})\to h_{B}(A)$ and $\gamma:h_{B}(A)\to \mathsf{Set}^\mathsf{C}(h_{A},h_{B})$ defined as $$\phi(\alpha)=\alpha_{A}(\text{id}_{A})\wedge \gamma(f)=\{s_{X\to A}\mapsto[h_{B}(s)](f)\}_{X\in \text{Ob}(\mathsf{C})}$$are isomorphisms and inverses of each other. We will first show that for all morphisms $f:A\to B$, $\gamma(f)=h_{f}$.

Suppose $X$ is an object in $\mathsf{C}$. Suppose $s:X\to A$ is a morphism in $\mathsf{C}$. We have
$$\begin{align}
[\gamma(f)_{X}](s) & =[h_{B}(s)](f) \\
 & =f\circ s \\
 & =(h_{f})_{X}(s).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $\gamma(f)=h_{f}$.

We now show that for all natural transformations $\alpha:h_{A}\Rightarrow h_{B}$ there is a unique morphism $f:A\to B$ such that $h_{f}=\alpha$; this then proves that $h_{\bullet}$ is full and faithful.
Suppose $\alpha:h_{A}\Rightarrow h_{B}$.
- **Existence.** We pick $f=\phi(\alpha)$. Since $\phi$ and $\gamma$ are inverses, $$h_{f}=\gamma(f)=\gamma(\phi(\alpha))=\alpha.$$
- **Uniqueness.** Suppose $f:A\to B$ and $g:A\to B$ satisfy $h_{f}=\alpha$ and $h_{g}=\alpha$. Then, $h_{f}=h_{g}$, so $\gamma(f)=\gamma(g)$. This means $$\phi(\gamma(f))=\phi(\gamma(g)),$$so, since $\phi$ and $\gamma$ are inverses, $f=g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Faithful Functor]]
- [[Full Functor]]
- [[Functor Category]]
- [[Hom-Functor]]
- [[Natural Transformation Between Hom-Functors]]
- [[Yoneda Embedding]]
- [[Bijective Function]]
- [[Category of Sets]]

Theorems used:
- [[Yoneda Lemma]]
- [[Extensionality of Functions]]
- [[Bijective Functions as Isomorphisms]]