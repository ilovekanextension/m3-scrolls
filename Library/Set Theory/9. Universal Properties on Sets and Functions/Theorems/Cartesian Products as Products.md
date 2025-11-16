**Theorem.** Let $A$ and $B$ be sets. Then, the Cartesian Product $A\times B$ together with the projection functions $\pi_{1}:A\times B\to A$ and $\pi_{2}:A\times B\to B$ defined as $$\pi_{1}(a,b)=a\wedge \pi_{2}(a,b)=b$$is the product of $A$ and $B$.

**Proof.** Suppose $P$ is a set, and suppose we have functions $f:P\to A$ and $g:P\to B$. We need to show that there is a unique function $P\to A\times B$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[row sep=large]
 & P & \\
A & A\times B & B
\arrow[from=1-2, to=2-2]
\arrow["f", from=1-2, to=2-1, swap]
\arrow["g", from=1-2, to=2-3]
\arrow["\pi_1", from=2-2, to=2-1]
\arrow["\pi_2", from=2-2, to=2-3, swap]
\end{tikzcd}
\end{document}
```

commutes.
- **Existence.** Define a function $k:P\to A\times B$ as $$k(x)=(f(x),g(x)).$$To show that $k$ makes the diagram commute, suppose $x\in P$. Notice that, by [[Evaluations of Composite Functions]], $$\pi_{1}\circ k(x)=\pi_{1}(f(x),g(x))=f(x)$$and $$\pi_{2}\circ k(x)=\pi_{2}(f(x),g(x))=g(x).$$Therefore, by [[Extensionality of Functions]] $\pi_{1}\circ k=f$ and $\pi_{2}\circ k=g$.
- **Uniqueness.** Suppose $h:P\to A\times B$ makes the diagram commute. We need to show that $h=k$. By [[Extensionality of Functions]], it is then enough to show that $h(x)=k(x)$ for all $x\in P$.
  
  Suppose $x\in P$. For clarity, suppose $h(x)=(a,b)$, where $a\in A$ and $b\in B$. Since $h$ makes the diagram commute, $\pi_{1}\circ h=f$. In particular, this means $$\pi_{1}(h(x))=\pi_{1}\circ h(x)=f(x).$$Thus, $\pi_{1}(a,b)=f(x)$, so $a=f(x)$. Also, $\pi_{2}\circ h=g$, so in particular $$\pi_{2}(h(x))=\pi_{2}\circ h(x)=g(x).$$Thus, $\pi_{2}(a,b)=g(x)$, so $b=g(x)$. This means $$h(x)=(f(x),g(x))=k(x).\blacksquare$$

***
Definitions used:
- [[Set]]
- [[Cartesian Product]]
- [[Function]]
- [[Category of Sets]]
- [[Categorical Product]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]