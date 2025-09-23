**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Then, $$\sigma*\nu=K\nu\circ \sigma F$$or equivalently $$\sigma*\nu=\sigma G\circ H\nu.$$
**Proof.** Suppose $a$ is an object in $\mathsf{C}$. By definition, $(\sigma*\nu)_{a}=K(\nu_{a})\circ \sigma_{F(a)}$. Since $K(\nu_{a})=(K\nu)_{a}$ and $\sigma_{F(a)}=(\sigma F)_{a}$, we have $$(\sigma*\nu)_{a}=(K\nu)_{a}\circ(\sigma F)_{a}=(K\nu\circ \sigma F)_{a}.$$Therefore, $\sigma*\nu=K\nu\circ \sigma F$.

By [[Equivalence of Components of Horizontal Composites]], we have $$K(\nu_{a})\circ \sigma_{F(a)}=\sigma_{G(a)}\circ H(\nu_{a}).$$Therefore, $\sigma*\nu=\sigma G\circ H\nu$. $\blacksquare$
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