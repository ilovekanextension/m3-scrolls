**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let the following be a pair of adjunctions.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C} & \mathsf{D} & \mathsf{E}
\arrow["F"{name=F}, from=1-1, to=1-2, bend left=25]
\arrow["G"{name=G}, from=1-2, to=1-1, bend left=25]
\arrow["H"{name=H}, from=1-2, to=1-3, bend left=25]
\arrow["K"{name=K}, from=1-3, to=1-2, bend left=25]
\arrow["\perp", phantom, from=F, to=G]
\arrow["\perp", phantom, from=H, to=K]
\end{tikzcd}
\end{document}
```

Then, $H\circ F\dashv G\circ K$. Visually, we have the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C} & \mathsf{E}
\arrow["H\circ F"{name=HF}, from=1-1, to=1-2, bend left=25]
\arrow["G\circ K"{name=GK}, from=1-2, to=1-1, bend left=25]
\arrow["\perp", phantom, from=HF, to=GK]
\end{tikzcd}
\end{document}
```

**Proof.** Suppose $C$ and $E$ are objects in $\mathsf{C}$ and $\mathsf{E}$ respectively. Since $F\dashv G$, there is an isomorphism $$f:\mathsf{D}(F(C),K(E))\cong \mathsf{C}(C,G(K(E)))$$natural in both variables. Since $H\dashv K$, there is also an isomorphism $$g:\mathsf{E}(H(F(C)),E)\cong \mathsf{D}(F(C),K(E))$$natural in both variables. By [[Isomorphism Relation as Equivalence Relation]], we have an isomorphism $$f\circ g:\mathsf{E}(H\circ F(C),E)\cong\mathsf{C}(C,G\circ K(E)).$$This isomorphism is clearly natural in both variables. $\blacksquare$

