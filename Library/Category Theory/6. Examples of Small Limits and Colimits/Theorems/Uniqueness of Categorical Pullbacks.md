Let $\mathsf{C}$ be a category. Let $a,b,$ and $c$ be objects in $\mathsf{C}$. Let $f:a\to c$ and $g:b\to c$ be morphisms in $\mathsf{C}$. A **pullback** of $f$ and $g$ consists of
- an object $p$,
- a morphism $\phi_{1}:p\to a$, and
- a morphism $\phi_{2}:p\to b$

such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
p & a \\
b & c
\arrow["\phi_1", from=1-1, to=1-2]
\arrow["\phi_2", from=1-1, to=2-1, swap]
\arrow["g", from=2-1, to=2-2]
\arrow["f", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes and for all objects $q$ and morphisms $x:q\to a$ and $y:q\to b$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
q & a \\
b & c
\arrow["x", from=1-1, to=1-2]
\arrow["y", from=1-1, to=2-1, swap]
\arrow["g", from=2-1, to=2-2]
\arrow["f", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commute, there is a unique morphism $k:q\to p$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & q & \\
b & p & a
\arrow["k" description, from=1-2, to=2-2]
\arrow["\phi_2", from=2-2, to=2-1]
\arrow["\phi_1", from=2-2, to=2-3, swap]
\arrow["y", from=1-2, to=2-1, swap]
\arrow["x", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes.

**Theorem.** Let $\mathsf{C}$ be a category. Let $a,b,$ and $c$ be objects in $\mathsf{C}$. Let $f:a\to c$ and $g:b\to c$ be morphisms in $\mathsf{C}$. Suppose that $(p,\phi_{1}:p\to a,\phi_{2}:p\to b)$ and $(q,\eta:q\to a,\eta_{2}:q\to b)$ are pullbacks of $f$ and $g$. Then, $p\cong q$.

In fact, the isomorphism $p\cong q$ such that the diagram 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
b & q & a
\arrow["\cong" description, from=1-2, to=2-2]
\arrow["y", from=2-2, to=2-1]
\arrow["x", from=2-2, to=2-3, swap]
\arrow["\phi_2", from=1-2, to=2-1, swap]
\arrow["\phi_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes is unique, so pullbacks are actually unique up to **unique** isomorphism.

**Proof.** Since $p$ and $q$ are both pullbacks, by commutativity of the pullback morphisms we have $f\circ\phi_{1}=g\circ \phi_{2}$ and $f\circ \eta_{1}=g\circ \eta_{2}$. Since $p$ is a pullback and we have morphisms $\eta_{1}:q\to a$ and $\eta_{2}:q\to b$, there is a morphism $k:q\to p$ such that the diagram (hereafter denoted as (1)) 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & q & \\
b & p & a
\arrow["k" description, from=1-2, to=2-2]
\arrow["\phi_2", from=2-2, to=2-1]
\arrow["\phi_1", from=2-2, to=2-3, swap]
\arrow["\eta_2", from=1-2, to=2-1, swap]
\arrow["\eta_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes. Likewise, since $q$ is a pullback and we have morphisms $\phi_{1}:p\to a$ and $\phi_{2}:p\to b$, there is a morphism $\ell:p\to q$ such that the diagram (hereafter denoted as (2))

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
b & q & a
\arrow["\ell" description, from=1-2, to=2-2]
\arrow["\eta_2", from=2-2, to=2-1]
\arrow["\eta_1", from=2-2, to=2-3, swap]
\arrow["\phi_2", from=1-2, to=2-1, swap]
\arrow["\phi_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes. Consider the morphism $k\circ \ell:p\to p$. By commutativity of $(1)$, $\eta_{1}=\phi_{1}\circ k$ and $\eta_{2}=\phi_{2}\circ k$. By commutativity of $(2)$, $\phi_{1}=\eta_{1}\circ\ell$ and $\phi_{2}=\eta_{2}\circ\ell$. Therefore, $\phi_{1}=\phi_{1}\circ k\circ \ell$ and $\phi_{2}=\phi_{2}\circ k\circ \ell$, so the diagram (hereafter denoted as (3))

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
b & p & a
\arrow["k\circ \ell" description, from=1-2, to=2-2]
\arrow["\phi_2", from=2-2, to=2-1]
\arrow["\phi_1", from=2-2, to=2-3, swap]
\arrow["\phi_2", from=1-2, to=2-1, swap]
\arrow["\phi_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes. The following diagram (hereafter denoted as (4)) also commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
b & p & a
\arrow["\text{id}_p" description, from=1-2, to=2-2]
\arrow["\phi_2", from=2-2, to=2-1]
\arrow["\phi_1", from=2-2, to=2-3, swap]
\arrow["\phi_2", from=1-2, to=2-1, swap]
\arrow["\phi_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

Since $p$ is a pullback, the morphism $p\to p$ making the diagram commute must be unique. Therefore, by commutativity of (3) and (4), we have $k\circ\ell=\text{id}_{p}$. By the same reasoning, $\ell\circ k=\text{id}_{q}$. This means $k$ is an isomorphism with inverse $\ell$, so $p\cong q$.

Now suppose $k_{1}:p\to q$ and $k_{2}:p\to q$ are isomorphisms making the diagram posed in the statement commutes. Since $q$ is a pullback, we must have $k_{1}=k_{2}$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Categorical Diagram]]