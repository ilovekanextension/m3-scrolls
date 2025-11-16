**Theorem.** Let $A$ and $B$ be sets. Let $g:\mathcal{P}(B)\to\mathcal{P}(A)$, and suppose that for all families $F:I\to\mathcal{P}(B)$ of subsets of $B$ we have $$g\left(\bigcup_{\alpha\in I}F_{\alpha}\right)=\bigcup_{\alpha\in I}g(F_{\alpha})$$and $$g\left(\bigcap_{\alpha\in I}F_{\alpha}\right)=\bigcap_{\alpha\in I}g(F_{\alpha}).$$
1. We have $g(\varnothing)=\varnothing$ and $g(B)=A$.
2. There is a unique function $f:A\to B$ such that $g=f^{-1}[{-}]$.

**Proof of First Statement.** Consider the empty family $F:\varnothing\to\mathcal{P}(A)$. First, notice that, since $\varnothing$ is empty,
$$\begin{align}
\bigcup_{\alpha\in I}F_{\alpha} & =\{x\in B\mid \exists \alpha\in I \ (x\in F_{\alpha})\} \\
 & =\{x\in B\mid \exists \alpha\in\varnothing \ (x\in F_{\alpha})\} \\
 & =\varnothing
\end{align}$$
and
$$\begin{align}
\bigcup_{\alpha\in I}g(F_{\alpha}) & =\{x\in A\mid \exists \alpha\in I \ (x\in g(F_{\alpha}))\} \\
 & =\{x\in A\mid \exists \alpha\in\varnothing \ (x\in g(F_{\alpha}))\} \\
 & =\varnothing.
\end{align}$$
By the union property of $g$, we then must have $g(\varnothing)=\varnothing$. Next, notice that, since $\varnothing$ is empty,
$$\begin{align}
\bigcap_{\alpha\in I}F_{\alpha} & =\{x\in B\mid \forall x\in I \ (x\in F_{\alpha})\} \\
 & =\{x\in B\mid \forall x\in \varnothing \ (x\in F_{\alpha})\} \\
 & =B
\end{align}$$
and
$$\begin{align}
\bigcap_{\alpha\in I}g(F_{\alpha}) & =\{x\in A\mid \forall x\in I \ (x\in g(F_{\alpha}))\} \\
 & =\{x\in A\mid \forall x\in \varnothing \ (x\in g(F_{\alpha}))\} \\
 & =A.
\end{align}$$
By the intersection property of $g$, we then must have $g(A)=B$. $\blacksquare$

**Proof of Second Statement.** We will first show that for all $a\in A$ there is a unique $b\in B$ such that $a\in g(\{b\})$. Suppose $a\in A$.
- **Existence.** By the first statement, $g(B)=A$. Since $a\in A$, this means $a\in g(B)$. By [[Sets as Unions of Singletons]], $$B=\bigcup_{b\in B}\{b\}.$$Since $a\in g(B)$, this means $a\in g(\bigcup_{b\in B}\{b\})$, so by the union property of $g$ we have $a\in\bigcup_{b\in B}g(\{b\})$. Therefore, there is $b\in B$ such that $a\in g(\{b\})$.
- **Uniqueness.** Suppose $b\in B$ and $c\in B$, and suppose that $a\in g(\{b\})$ and $a\in g(\{c\})$. By the intersection property of $g$, $$g(\{b\}\cap\{c\})=g(\{b\})\cap g(\{c\}).$$Since $a\in g(\{b\})$ and $a\in g(\{c\})$, we have $a\in g(\{b\})\cap g(\{c\})$, so $a\in g(\{b\}\cap\{c\})$. This means $g(\{b\}\cap\{c\})$ is nonempty. Now assume for the sake of contradiction that $\{b\}\cap\{c\}=\varnothing$. Then, since $g(\varnothing)=\varnothing$, we have $g(\{b\}\cap\{c\})=\varnothing$, so $g(\{b\})\cap g(\{c\})=\varnothing$. However, $a\in g(\{b\})\cap g(\{c\})$, so $a\in\varnothing$. This contradicts the fact that $\varnothing$ is empty. Therefore, the assumption that $\{b\}\cap\{c\}$ is empty must be false, so $\{b\}\cap\{c\}$ is nonempty. Thus, there is $x\in B$ such that $x\in\{b\}$ and $x\in\{c\}$. This means $x=b$ and $x=c$, so $b=c$.

We can therefore construct a function $f:A\to B$ that maps $a\in A$ to the unique $b\in B$ such that $a\in g(\{b\})$. We will first show that $g=f^{-1}[{-}]$. By [[Extensionality of Functions]], it is enough to show that $g(X)=f^{-1}[X]$ for all $X\subseteq B$. Suppose $X\subseteq B$. By [[Sets as Unions of Singletons]], $$X=\bigcup_{x\in X}\{x\}.$$Thus, by the union property of $g$,
$$\begin{align}
g(X) & =g\left(\bigcup_{x\in X}\{x\}\right) \\
 & =\bigcup_{x\in X}g(\{x\}) \\
 & =\{a\in A\mid \exists x\in X \ (a\in g(\{x\}))\} \\
 & =\{a\in A\mid \exists x\in X \ (f(a)=x)\} \\
 & =\{a\in A\mid f(a)\in X\} \\
 & =f^{-1}[X].
\end{align}$$

Now suppose $h:A\to B$, and suppose that $g=h^{-1}[{-}]$. To show that $f=h$, by [[Extensionality of Functions]] it is enough to show that $f(a)=h(a)$ for all $a\in A$. Suppose $a\in A$. By definition of $f$, $a\in g(\{f(a)\})$. Also, since $g=h^{-1}[{-}]$, by [[Extensionality of Functions]] $g(\{h(a)\})=h^{-1}[\{h(a)\}]$. By definition,
$$\begin{align}
h^{-1}[\{h(a)\}] & =\{b\in B\mid \exists x\in A \ (h(x)\in\{h(a)\})\} \\
 & =\{b\in B\mid \exists x\in A \ (h(x)=h(a))\},
\end{align}$$
so since $h(a)=h(a)$ we have $a\in h^{-1}[\{h(a)\}]$. Thus, $a\in g(\{h(a)\})$. By a previous uniqueness argument, since $a\in g(\{f(a)\})$ and $a\in g(\{h(a)\})$, we must have $f(a)=h(a)$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Empty Set]]
- [[Nonempty Set]]
- [[Set Builder Notation]]
- [[Function]]
- [[Preimage of Subset]]
- [[Family of Subsets]]
- [[Union of Family of Sets]]
- [[Intersection of Family of Sets]]