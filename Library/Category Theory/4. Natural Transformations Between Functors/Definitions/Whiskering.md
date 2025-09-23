**Definition.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories.
1. Let $H:\mathsf{C}\to \mathsf{D}$ and $F,G:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$. The **whiskering** of $H$ and $\nu$, denoted $\nu H$, is the horizontal composition of $\text{id}_{H}$ and $\nu$. Thus, $\nu H=\nu*\text{id}_{H}$, so for all objects $a$ in $\mathsf{C}$ we have $$(\nu H)_{a}=(\nu*\text{id}_{H})_{a}=\nu_{H(a)}.$$
2. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$. The **whiskering** of $\nu$ and $H$, denoted $H \nu$, is the horizontal composition of $\nu$ and $\text{id}_{H}$. Thus, $H \nu=\text{id}_{H}*\nu$, so for all objects $a$ in $\mathsf{C}$ we have $$(H \nu)_{a}=(\text{id}_{H}*\nu)_{a}=H(\nu_{a}).$$

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Horizontal Composition of Natural Transformations]]