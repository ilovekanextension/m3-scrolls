**Definition.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories.
1. Let $H:\mathsf{C}\to \mathsf{D}$ and $F,G:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$. The **whiskering** of $H$ and $\nu$, denoted $\nu H$, is the horizontal composition of $\text{id}_{H}$ and $\nu$. That is, we define $$\nu H=\nu*\text{id}_{H}.$$Therefore, for all objects $A$ in $\mathsf{C}$ we have $$(\nu H)_{A}=(\nu*\text{id}_{H})_{A}=\nu_{H(A)}.$$
2. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$. The **whiskering** of $\nu$ and $H$, denoted $H \nu$, is the horizontal composition of $\nu$ and $\text{id}_{H}$. That is, we define $$H\nu=\text{id}_{H}*\nu.$$Therefore, for all objects $A$ in $\mathsf{C}$ we have $$(H \nu)_{A}=(\text{id}_{H}*\nu)_{A}=H(\nu_{A}).$$

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Horizontal Composition of Natural Transformations]]