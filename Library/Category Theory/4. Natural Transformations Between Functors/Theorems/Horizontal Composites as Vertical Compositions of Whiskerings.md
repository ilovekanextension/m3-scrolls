**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Then, $$\sigma*\nu=K\nu\circ \sigma F$$or equivalently $$\sigma*\nu=\sigma G\circ H\nu.$$
**Proof.** Suppose $A$ is an object in $\mathsf{C}$. By definition, $(\sigma*\nu)_{A}=K(\nu_{A})\circ \sigma_{F(A)}$. Since $K(\nu_{A})=(K\nu)_{A}$ and $\sigma_{F(A)}=(\sigma F)_{A}$, we have $$(\sigma*\nu)_{A}=(K\nu)_{A}\circ(\sigma F)_{A}=(K\nu\circ \sigma F)_{A}.$$Therefore, $\sigma*\nu=K\nu\circ \sigma F$.

By [[Equivalence of Components of Horizontal Composites]], we have $$K(\nu_{A})\circ \sigma_{F(A)}=\sigma_{G(A)}\circ H(\nu_{A}).$$Therefore, $\sigma*\nu=\sigma G\circ H\nu$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]
- [[Horizontal Composition of Natural Transformations]]
- [[Whiskering]]

Theorems used:
- [[Equivalence of Components of Horizontal Composites]]