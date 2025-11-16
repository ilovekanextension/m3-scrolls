**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$ and $g:A\to B$. Then, the set $$E=\{a\in A\mid f(a)=g(a)\}$$together with the inclusion function $i:E\subseteq A$ is the equalizer of $f$ and $g$.

**Proof.** We will first show that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
E & A & B
\arrow["i", from=1-1, to=1-2]
\arrow["f", from=1-2, to=1-3, shift left]
\arrow["g", from=1-2, to=1-3, shift right, swap]
\end{tikzcd}
\end{document}
```

commutes. Suppose $a\in E$. Then, by definition $f(a)=g(a)$. Since $i(a)=a$, by [[Evaluations of Composite Functions]] this means $$f\circ i(a)=f(i(a))=f(a)=g(a)=g(i(a))=g\circ i(a).$$By [[Extensionality of Functions]], we can conclude that the diagram commutes.

Now suppose $P$ is an object equipped with a function $m:P\to A$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
P & A & B
\arrow["m", from=1-1, to=1-2]
\arrow["f", from=1-2, to=1-3, shift left]
\arrow["g", from=1-2, to=1-3, shift right, swap]
\end{tikzcd}
\end{document}
```

commutes. We will show that there is a unique function $P\to E$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
P \\
E & A
\arrow[from=1-1, to=2-1]
\arrow["i", from=2-1, to=2-2, swap]
\arrow["m", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.