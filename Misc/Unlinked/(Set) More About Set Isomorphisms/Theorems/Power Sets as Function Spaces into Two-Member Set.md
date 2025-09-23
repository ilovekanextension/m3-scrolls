*Theorem.* Let $A$ be a set. Let $2$ be the set $\{0,1\}$. Then, the power set $\mathcal{P}(A)$ of $A$ is isomorphic to the function space $2^A$. That is, $$\mathcal{P}(A)\cong 2^A.$$
*Proof.* Define a function $f:\mathcal{P}(A)\to 2^A$ as follows: $$f(X)=f_{X}$$is the function $A\to 2$ defined by $$f_{X}(a)=\begin{cases}
1, & a\in X, \\
0, & a\notin X.
\end{cases}$$We will show that $f$ is bijective; the statement in the theorem follows immediately.
- *Injectivity.* Suppose $X,Y\in\mathcal{P}(A)$, and suppose that $f(X)=f(Y)$. We will show that $X=Y$ by showing that $X\subseteq Y$ and $Y\subseteq X$.
  
  First suppose $x\in X$. Then, by definition of $f$, we have $f_{X}(x)=1$. Since $f(X)=f(Y)$, by [[Extensionality of Functions]] we must have $f_{X}(x)=f_{Y}(x)$, so $f_{Y}(x)=1$. This means $x\in Y$.
  
  Next suppose $y\in Y$. Then, by definition of $f$, we have $f_{Y}(y)=1$. Since $f(X)=f(Y)$, by [[Extensionality of Functions]] we must have $f_{X}(x)=f_{Y}(x)$, so $f_{X}(y)=1$. This means $y\in X$.
- *Surjectivity.* Suppose $g:A\to 2$ is a function. Define $X$ as the set $$X=\{a\in A\mid g(a)=1\}.$$Clearly $X\subseteq A$, so $X\in\mathcal{P}(A)$. Moreover, for all $a\in A$ we have $g(a)=1$ if and only if $a\in X$, so $$f_{X}(a)=\begin{cases}
1, & a\in X \\
0, & a\notin X
\end{cases}\ =\begin{cases}
1, & g(a)=1 \\
0, & g(a)=0
\end{cases}\ =g(a).$$By [[Extensionality of Functions]], this means $f_{X}=g$, so $f(X)=g$. $\blacksquare$