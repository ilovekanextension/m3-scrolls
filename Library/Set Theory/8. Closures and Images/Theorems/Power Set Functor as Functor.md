**Theorem.** The map $F$ that assigns
- to each set $A$ the power set $\mathcal{P}(A)$ and
- to each function $f:A\to B$ the preimage function $f^{-1}[{-}]:\mathcal{P}(B)\to\mathcal{P}(A)$

is a functor from $\mathsf{Set}^\text{op}$ to $\mathsf{Set}$.

**Proof.** First suppose $A$ is a set. To prove that $F(\text{id}_{A})=\text{id}_{F(A)}$, by definition of $F$ we need to show that $\text{id}_{A}^{-1}[{-}]=\text{id}_{\mathcal{P}(A)}$. Observe that for all $X\subseteq A$,
$$\begin{align}
\text{id}_{A}^{-1}[X] & =\{x\in A\mid \text{id}_{A}(x)\in X\} \\
 & =\{x\in A\mid x\in X\} \\
 & =X \\
 & =\text{id}_{\mathcal{P}(A)}(X),
\end{align}$$
so by [[Extensionality of Functions]] $\text{id}_{A}^{-1}[{-}]=\text{id}_{\mathcal{P}(A)}$.

Next suppose $f:A\to B$ and $g:B\to C$. To prove that $F(g\circ f)=F(f)\circ F(g)$, by definition of $F$ we need to show that $[g\circ f]^{-1}[{-}]=f^{-1}[{-}]\circ g^{-1}[{-}]$. Observe that for all $X\subseteq C$, by [[Evaluations of Composite Functions]],
$$\begin{align}
[g\circ f]^{-1}[X] & =\{x\in A\mid g\circ f(x)\in X\} \\
 & =\{x\in A\mid g(f(x))\in X\} \\
 & =\{x\in A\mid f(x)\in g^{-1}[X]\} \\
 & =\{x\in A\mid x\in f^{-1}[g^{-1}[X]]\} \\
 & =f^{-1}[g^{-1}[X]] \\
 & =[f^{-1}[{-}]\circ g^{-1}[{-}]](X),
\end{align}$$
so by [[Extensionality of Functions]] $[g\circ f]^{-1}[{-}]=f^{-1}[{-}]\circ g^{-1}[{-}]$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Function]]
- [[Category of Sets]]
- [[Preimage of Subset]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]