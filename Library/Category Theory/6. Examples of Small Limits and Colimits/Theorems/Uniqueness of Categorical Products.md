Let $\mathsf{C}$ be a category. Let $a$ and $b$ be objects in $\mathsf{C}$. A **product** of $a$ with $b$ consists of
- an object $p$,
- a morphism $\pi_{1}:p\to a$, and
- a morphism $\pi_{2}:p\to b$

such that for all objects $x$ and morphisms $f:x\to a$ and $g:x\to b$, there is a unique morphism $k:x\to p$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & x & \\
a & p & b
\arrow["k" description, from=1-2, to=2-2]
\arrow["\pi_1", from=2-2, to=2-1]
\arrow["\pi_2", from=2-2, to=2-3, swap]
\arrow["f", from=1-2, to=2-1, swap]
\arrow["g", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes.

**Theorem.** Let $\mathsf{C}$ be a category. Let $a$ and $b$ be objects in $\mathsf{C}$. Suppose that $(p,\pi_{1}:p\to a,\pi_{2}:p\to b)$ and $(q,\sigma_{1}:q\to a,\sigma_{2}:q\to b)$ are products of $a$ with $b$. Then, $p\cong q$. Hence, products are unique up to isomorphism.

In fact, the isomorphism $p\cong q$ such that the diagram 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
a & q & b
\arrow["\cong" description, from=1-2, to=2-2]
\arrow["\sigma_1", from=2-2, to=2-1]
\arrow["\sigma_2", from=2-2, to=2-3, swap]
\arrow["\pi_1", from=1-2, to=2-1, swap]
\arrow["\pi_2", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes is unique, so products are actually unique up to **unique** isomorphism.

**Proof.** Since $p$ is a product, there is a morphism $k:q\to p$ such that the following diagram (hereafter denoted as (1)) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & q & \\
a & p & b
\arrow["k" description, from=1-2, to=2-2]
\arrow["\pi_1", from=2-2, to=2-1]
\arrow["\pi_2", from=2-2, to=2-3, swap]
\arrow["\sigma_1", from=1-2, to=2-1, swap]
\arrow["\sigma_2", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

Likewise, since $q$ is a product, there is a morphism $\ell:p\to q$ such that the following diagram (hereafter denoted as (2)) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
a & q & b
\arrow["\ell" description, from=1-2, to=2-2]
\arrow["\sigma_1", from=2-2, to=2-1]
\arrow["\sigma_2", from=2-2, to=2-3, swap]
\arrow["\pi_1", from=1-2, to=2-1, swap]
\arrow["\pi_2", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

We will show that $k$ is an isomorphism with inverse $\ell$.

By commutativity of (1), $\pi_{1}\circ k=\sigma_{1}$ and $\pi_{2}\circ k=\sigma_{2}$. By commutativity of (2), $\sigma_{1}\circ \ell=\pi_{1}$ and $\sigma_{2}\circ \ell=\pi_{2}$. Substituting equalities from (2) to (1) gives $\sigma_{1}\circ (\ell\circ k)=\sigma_{1}$ and $\sigma_{2}\circ(\ell\circ k)=\sigma_{2}$. This means that the following diagram (hereafter denoted as (3)) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & q & \\
a & q & b
\arrow["\ell\circ k" description, from=1-2, to=2-2]
\arrow["\sigma_1", from=2-2, to=2-1]
\arrow["\sigma_2", from=2-2, to=2-3, swap]
\arrow["\sigma_1", from=1-2, to=2-1, swap]
\arrow["\sigma_2", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

The following diagram (hereafter denoted as (4)) also commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & q & \\
a & q & b
\arrow["\text{id}_q" description, from=1-2, to=2-2]
\arrow["\sigma_1", from=2-2, to=2-1]
\arrow["\sigma_2", from=2-2, to=2-3, swap]
\arrow["\sigma_1", from=1-2, to=2-1, swap]
\arrow["\sigma_2", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

Since $q$ is a product, the morphism $q\to q$ making the diagram commute is unique. Therefore, from commutativity of (3) and (4) we must have $\ell\circ k=\text{id}_{q}$. By a similar reasoning, substituting equalities from (1) to (2) gives $k\circ \ell=\text{id}_{p}$. This means $k$ is an isomorphism with inverse $\ell$, so $p\cong q$.

Now suppose $f:p\to q$ and $g:p\to q$ are isomorphisms making the diagram posed in the statement commutes. Then, since $q$ is a product, we must have $f=g$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Categorical Diagram]]