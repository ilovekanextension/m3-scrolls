**Theorem.** Let $A$ and $B$ be sets. Let $0$ and $1$ be distinct objects. Define $$A+B=(A\times \{0\})\cup (B\times\{1\}).$$Then, $A+B$ together with the insertion functions $\iota_{A}:A\to A+B$ and $\iota_{B}:B\to A+B$ defined as $$\iota_{A}(a)=(a,0)\wedge \iota_{B}(b)=(b,1)$$is the coproduct of $A$ and $B$. We call $A+B$ as the **disjoint union** of $A$ and $B$.

**Proof.** Suppose $C$ is a set, and suppose that we have functions $f:A\to C$ and $g:B\to C$. We will show that there is a unique function $A+B\to C$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[row sep=large]
A & A+B & B \\
 & C &
\arrow[from=1-2, to=2-2]
\arrow["f", from=1-1, to=2-2, swap]
\arrow["g", from=1-3, to=2-2]
\arrow["\iota_A", from=1-1, to=1-2]
\arrow["\iota_B", from=1-3, to=1-2, swap]
\end{tikzcd}
\end{document}
```

commutes.

Since $0$ and $1$ are distinct, there is no pair $(x,n)\in A+B$ such that $(x,n)\in A\times\{0\}$ and $(x,n)\in B\times\{1\}$. Thus, we can construct a well-defined function $k:A+B\to C$ as
$$k(x,n)=\begin{cases}
f(x) & n=0, \\
g(x) & n=1.
\end{cases}$$
- **Existence.** We will show by [[Extensionality of Functions]] that $k$ makes the diagram commute.
  
  First suppose $a\in A$. Then, by [[Evaluations of Composite Functions]], $$k\circ\iota_{A}(a)=k(\iota_{A}(a))= k(a,0)=f(a).$$We can conclude that $k\circ\iota_{A}=f$. Next suppose $b\in B$. Then, by [[Evaluations of Composite Functions]], $$k\circ\iota_{B}(b)=k(\iota_{B}(b))=k(b,1)=g(b).$$We can conclude that $k\circ\iota_{B}=g$. Overall, this means $k$ makes the diagram commute.
- **Uniqueness.** Suppose $h:A+B\to C$ makes the diagram commute. We need to show that $h=k$. By [[Extensionality of Functions]], it is then enough to show that $h(x,n)=k(x,n)$ for all $(x,n)\in A+B$.
  
  Suppose $(x,n)\in A+B$. By definition of $A+B$, we have $n=0$ or $n+1$. We proceed by cases; in each case we will show that $h(x,n)=k(x,n)$.
	- **Case** $n=0$. This means $(x,n)=(x,0)$, so $x\in A$. Since $h$ makes the diagram commute, we have $h\circ\iota_{A}=f$. In particular, this means $$h(\iota_{A}(x))=f(x),$$so $h(x,0)=f(x)$. Since by definition $k(x,0)=f(x)$, we can conclude that $h(x,0)=k(x,0)$.
	- **Case** $n=1$. This means $(x,n)=(x,1)$, so $x\in B$. Since $h$ makes the diagram commute, we have $h\circ\iota_{B}=g$. In particular, this means $$h(\iota_{B}(x))=g(b),$$so $h(x,1)=g(x)$. Since by definition $k(x,1)=g(x)$, we can conclude that $h(x,1)=k(x,1)$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Singleton]]
- [[Union of Two Sets]]
- [[Cartesian Product]]
- [[Function]]
- [[Category of Sets]]
- [[Categorical Coproduct]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]