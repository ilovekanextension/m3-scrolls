**Theorem.** Let $\mathsf{C}$ be a locally small category. Then, the Yoneda embeddings $h^{\bullet}:\mathsf{C}^\text{op}\to \mathsf{Set}^\mathsf{C}$ and $h_{\bullet}:\mathsf{C}\to \mathsf{Set}^{\mathsf{C}^\text{op}}$ are full and faithful.

**Proof of First Statement.** Suppose $a$ and $b$ are objects in $\mathsf{C}$. By [[Yoneda Lemma]], the map $$\Gamma:\mathsf{C}^\text{op}(a,b)=h^b(a)\to \mathsf{Set}^\mathsf{C}(h^a,h^b)$$defined as $\Gamma(f)_{x}(s)=h^b(s)(f)$ is well-defined and bijective with inverse $$\Phi:\mathsf{Set}^\mathsf{C}(h^a,h^b)\to h^b(a)$$defined as $\Phi(\alpha)=\alpha_{a}(\text{id}_{a})$. We will show that $\Gamma$ is equal to the restricted map $h^{\bullet}:\mathsf{C}^\text{op}(a,b)\to \mathsf{Set}^\mathsf{C}(h^a,h^b)$; this will imply that the restricted map $h^{\bullet}$ is bijective, thereby showing that $h^{\bullet}$ is full and faithful.

Suppose $f:b\to a$. We have $$\Phi(h^f)=(h^f)_{a}(\text{id}_{a})=\text{id}_{a}\circ f=f.$$Since $\Gamma$ is bijective with inverse $\Phi$, we have $\Gamma(\Phi(h^f))=h^f$. Therefore, $$(h^{\bullet})(f)=h^f=\Gamma(\Phi(h^f))=\Gamma(f).$$By [[Extensionality of Functions]], this means $\Gamma=h^{\bullet}$. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$
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
- [[Principle of Duality]]
- [[Yoneda Lemma]]
- [[Extensionality of Functions]]
- [[Bijective Functions as Isomorphisms]]