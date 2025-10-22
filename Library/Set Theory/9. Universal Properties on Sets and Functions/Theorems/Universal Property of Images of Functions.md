**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Let $i: \text{im}(f)\hookrightarrow B$ be the inclusion function. Then, there is a function $e:A\to \text{im}(f)$ such that $f=i\circ e$. Moreover, for all $m:X\hookrightarrow B$ and $g:A\to X$ satisfying $$f=m\circ g$$there exists a unique function $v: \text{im}(f)\to v$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \text{im}(f) & B \\
 & X & 
\arrow["e", from=1-1, to=1-2]
\arrow["i", from=1-2, to=1-3, hook]
\arrow["g", from=1-1, to=2-2, swap]
\arrow["m", from=2-2, to=1-3, hook, swap]
\arrow["v", from=1-2, to=2-2, dashed]
\end{tikzcd}
\end{document}
```

commutes.

**Proof of First Statement.** Define a function $e:A\to \text{im}(f)$ as $e(a)=f(a)$. By [[Evaluations of Composite Functions]], for all $a\in A$ we have $$i\circ e(a)=i(e(a))=e(a)=f(a).$$Therefore, by [[Extensionality of Functions]] $i\circ e=f$.

**Proof of Second Statement.** Suppose $m:X\hookrightarrow B$ and $g:A\to X$ satisfy $$f=m\circ g.$$We will first show that for all $a,b\in A$, if $f(a)=f(b)$, then $g(a)=g(b)$. Suppose $a,b\in A$ satisfy $f(a)=f(b)$. Since $f=m\circ g$, by [[Evaluations of Composite Functions]] we have
$$\begin{align}
m(g(a)) & =m\circ g(a) \\
 & =f(a) \\
 & =f(b) \\
 & =m\circ g(b) \\
 & =m(g(b)).
\end{align}$$
Since $m$ is injective, we must then have $g(a)=g(b)$.

- **Existence.** By the previous observation, we can construct a function $v:\text{im}(f)\to X$ defined as $$v(b)=g(a)$$whenever $b=f(a)$. We will show that $v$ makes the diagram commute. First suppose $b\in \text{im}(f)$. Then, there is $a\in A$ such that $b=f(a)$. By [[Evaluations of Composite Functions]], $$\begin{align}
m\circ v(b) & =m(v(b)) \\
 & =m(v(f(a))) \\
 & =m(g(a)) \\
 & =f(a) \\
 & =b \\
 & =i(b).
\end{align}$$Therefore, by [[Extensionality of Functions]] $m\circ v=i$. Next suppose $a\in A$. We have $$\begin{align}
v\circ e(a) & =v(e(a)) \\
 & =v(f(a)) \\
 & =g(a).
\end{align}$$Therefore, by [[Extensionality of Functions]] $v\circ e=g$.
- **Uniqueness.** Suppose $w:\text{im}(f)\to X$ makes the diagram commute. We will show that $w=v$. Suppose $b\in \text{im}(f)$. Then, there is $a\in A$ such that $b=f(a)$. Since $w$ makes the diagram commute, $w\circ e=g$. This means $$\begin{align}
w(b) & =w(f(a)) \\
 & =w(e(a)) \\
 & =w\circ e(a) \\
 & =g(a).
\end{align}$$Since $v(b)=v(f(a))=g(a)$, by [[Extensionality of Functions]] we can conclude that $w=v$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Composition of Functions]]
- [[Injective Function]]
- [[Inclusion Function]]
- [[Image of Function]]
- [[Categorical Diagram]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]