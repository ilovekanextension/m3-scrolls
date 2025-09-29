**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $f:X\to Y$ be a morphism in $\mathsf{C}$.
1. $f$ is an isomorphism if and only if $h^f:h^Y\Rightarrow h^X$ is a natural isomorphism. Therefore, $X\cong Y$ if and only if $h^X\cong h^Y$.
2. $f$ is an isomorphism if and only if $h_{f}:h_{X}\Rightarrow h_{Y}$ is a natural isomorphism. Therefore, $X\cong Y$ if and only if $h_{X}\cong h_{Y}$.

**Proof of First Statement.**
- **Forward Implication.** Suppose $f$ is an isomorphism. Since $h^\bullet$ is a functor, $$h^f\circ h^{f^{-1}}=h^{f^{-1}\circ f}=h^{\text{id}_{X}}=\text{id}_{h^X}$$and $$h^{f^{-1}}\circ h^f=h^{f\circ f^{-1}}=h^{\text{id}_{Y}}=\text{id}_{h^Y}.$$This means $h^f$ is an isomorphism with inverse $h^{f^{-1}}$. $\blacksquare$
- **Backward Implication.** Suppose $h^f$ is a natural isomorphism. Then, there is $(h^f)^{-1}:h^X\to h^Y$ such that $h^f\circ (h^f)^{-1}=\text{id}_{h^X}$ and $(h^f)^{-1}\circ h^f=\text{id}_{h^Y}$. By [[Fullness and Faithfulness of Yoneda Embeddings]], $h^{\bullet}$ is full and faithful. Since $h^\bullet$ is full, there is $g:Y\to X$ such that $(h^f)^{-1}=h^g$. This means $$h^{\text{id}_{Y}}=\text{id}_{h^Y}=h^g\circ h^f=h^{f\circ g}$$and $$h^{\text{id}_{X}}=\text{id}_{h^X}=h^f\circ h^g=h^{g\circ f},$$so, since $h^\bullet$ is faithful, $f\circ g=\text{id}_{Y}$ and $g\circ f=\text{id}_{X}$. This means $f$ is an isomorphism with inverse $g$. $\blacksquare$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $f$ is an isomorphism. Since $h_{\bullet}$ is a functor, $$h_f\circ h_{f^{-1}}=h_{f\circ f^{-1}}=h_{\text{id}_{Y}}=\text{id}_{h_{Y}}$$and $$h_{f^{-1}}\circ h_f=h_{f^{-1}\circ f}=h_{\text{id}_{X}}=\text{id}_{h_{Y}}.$$This means $h_{f}$ is an isomorphism with inverse $h_{f^{-1}}$. $\blacksquare$
- **Backward Implication.** Suppose $h_{f}$ is a natural isomorphism. Then, there is $(h_{f})^{-1}:h^Y\to h^X$ such that $h_{f}\circ (h_f)^{-1}=\text{id}_{h_Y}$ and $(h_f)^{-1}\circ h_{f}=\text{id}_{h_{X}}$. By [[Fullness and Faithfulness of Yoneda Embeddings]], $h_{\bullet}$ is full and faithful. Since $h_\bullet$ is full, there is $g:Y\to X$ such that $(h_f)^{-1}=h_g$. This means $$h_{\text{id}_{X}}=\text{id}_{h_X}=h_g\circ h_f=h_{g\circ f}$$and $$h_{\text{id}_{Y}}=\text{id}_{h_Y}=h_f\circ h_g=h_{f\circ g},$$so, since $h^\bullet$ is faithful, $g\circ f=\text{id}_{X}$ and $f\circ g=\text{id}_{Y}$. This means $f$ is an isomorphism with inverse $g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Locally Small Category]]
- [[Vertical Composition of Natural Transformations]]
- [[Natural Isomorphism]]
- [[Hom-Functor]]
- [[Natural Transformation Between Hom-Functors]]
- [[Yoneda Embedding]]

Theorems used:
- [[Fullness and Faithfulness of Yoneda Embeddings]]

